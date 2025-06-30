---
layout: default
---

# Methods

## Contents

- Methods
  - [Introduction](#introduction)
  - [Methods](#methods)
    - [Method Naming](#method-naming)
    - [Method Dispatch](#method-dispatch)
    - [Type checking](#type-checking)


## Introduction

This page contains basic information for coders on Methods.  


## Methods

In **SOZ** a Method is just a specialised form of a Function - able to be called in two ways:

- as a standard Function call.
- as a Method call - refer to [Method Dispatch](#method-dispatch) below.

All Methods for each Class / Object are written as pure function definitions, with an additional call to register the Method into the **Meta**.

Examples of method calls and definitions are:

```common-lisp
(SZMAMethod-make "SZGELine" "StartPoint" (list "O") (list "SZGELine") "Point" "StartPoint of a SZGELine")
(defun SZGELine-StartPoint (o) (Line-StartPoint (SZOB->line o)))

(SZMAMethod-make "SZGELine" "EndPoint" (list "O") (list "SZGELine") "Point" "EndPoint of a SZGELine")
(defun SZGELine-EndPoint (o) (Line-EndPoint (SZOB->line o)))

(SZMAMethod-make "SZGELine" "MidPoint" (list "O") (list "SZGELine") "Point" "MidPoint of a SZGELine")
(defun SZGELine-MidPoint (o) (SZGELine-BaryComb o 0.5))
```

where `SOZMethod-Make` has the following signature:

`(SZMAMethod-make ClassName MethodName Arg-Keys Arg-Types Returns Description)`

And:

| Item | Type | Description |
| --------- | --------- | --------- |
| ClassName | String | Name of the Class for the Method |
| MethodName | String | Name of the Method being created |
| Arg-Keys | List:Key | A list of the Keys required for the Method - or nil if none |
| Arg-Types | List:Types | A list of the Types required for the Method - or nil if none |
| Returns | Type | a Type returned by the Method |
| Description | Comment | a Description of the Method being created |



### Method Naming

Every Method, except for predicate functions, is consistently named as:

`(ClassName-MethodName Args)`

With predicate functions having the signature of:

`(ClassName? o)`

This structured approach to function naming has the immediate benefits of:

- code consistency
- code readability
- simple Method look-up and dispatch.
- class and method documentation


### Method Dispatch

One routine dispatches the methods for all classes:

```common-lisp
(SZMAClass-Apply ClassName MethodName Args)
```
And even the generic Object method dispatch routine, below is just a wrapper for the class apply function above.

```common-lisp
(defun SZOB-Apply (object MethodName Args / ClassName) 
  (if (and (setq ClassName (SZOB-getClass object)) (string? ClassName)) 
    (SZMAClass-Apply ClassName MethodName (cons object Args))))
```

That then translates into Lisp code as:

`(ClassName-MethodName (cons object Args))`

Where:

| Item | Description |
| --------- | --------- |
| class-method | is the function name called by Lisp  |
| class | is the class or type of object being processed |
| method | is the method name being invoked |
| (cons object args) | is a list created (using the cons function) of the arguments for the method. |
| object | is the object the method is being invoked on |
| args | is a list of the remaining arguments required for the method |



This approach enables class hierarchies to be traversed and method selection to be made easily.

Thereby reducing the number of functions to be written to a minimum.


### Type checking

Every method specifies the Type of each argument required and **SOZ** limits user inputs to the desired types at run-time.

By rigidly enforcing **LSP** principles, it is possible to ensure that user input will be suitable for **SOZ** to process.

