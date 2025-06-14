---
layout: default
---

# Coders Basics

## Contents

- Coders
  - [Introduction](#introduction)
  - [Classes](#classes)
  - [Objects](#objects)
  - [Methods](#methods)
    - [Method Naming](#method-naming)
    - [Method Dispatch](#method-dispatch)
    - [Type checking](#type-checking)
  - [Interfaces](#interfaces)
  - [Categories](#categories)
  - [Strings vs Symbols](#strings-vs-symbols)
  - [The Meta Environment](#the-meta-environment)
 

## Introduction

This page contains basic information for coders working with **SOZ**.  


## Classes

All classes are derived from the Base Class - **SZOBBase**.

While **SOZ** only uses single inheritance:

- Classes can share an interface with other classes.
- Classes can be contained in multiple Categories.

Each entry in the [Class Hierarchy](/repos/soz-live.html) is a link to the documentation for the particular class.

A class is defined with a call to register it in the [Meta Environment](#the-meta-environment) using the Class Make function:

```common-lisp
(SZMAClass-make "SZGECurve" "SZGELine" :vlax-false "Line Geometry Class")
```

Where the `SZMAClass-Make` function has the following signature:

`(SZMAClass-make BaseClass ClassName isAbstract? Description)`

And:

| Item | Type | Description |
| --------- | --------- | --------- |
| BaseClass | String | Name of the Base class for the Class |
| ClassName | String | Name of the Class being created |
| isAbstract? | Boolean | is the Class an Abstract Class |
| Description | Comment | a Description of the Class being created |

> **Notes:**<br>
> - Many of the specified classes are Abstract classes - meaning that they can't be instanced - or objects created from them.  
> - They are used to set out the hierarchy in a logical fashion so that LSP works for each type / class specified.


## Objects

All Objects are made using the Make method of the Class, as shown below:

```common-lisp
(SZMAMethod-make "SZGELine" "Make" (list "POINT0" "POINT1") (list "SZGEPoint" "SZGEPoint") "SZGELine" "Make a Line")
(defun SZGELine-make ( POINT0 POINT1 ) (SZOBObject-Maker "SZGELine" )) 
```

This differs to other Lisp OO implementations where a make routine for a **Line** class would be named **make-line**.

The Make arguments are stored on the Object or Entity in an Alist, together with the Class of the Object.
They contain all the information required to Make, Edit and Update the object as and if required.


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


## Interfaces

An Interface enables a class A to be used where class B would be required, as it contains the same method signatures as Class B.

```common-lisp
(SZMAInterface-make "AcDbPoint" (list "SZGEPoint" "Point"))
```

This then enables an AcDbPoint entity to be used interchangeably with either a SZGEPoint object or a Point value.  


Where `SZMAInterface-make` has the following signature:

`(SZMAInterface-make ClassName Classes)`

And:

| Item | Type | Description |
| --------- | --------- | --------- |
| ClassName | String | Name of the Class |
| Classes | List:ClassName | a list of Classes to Interface with |



## Categories

A Category can be considered an orthogonal concept to a Class.

Both have a hierarchy, and both only allow single inheritance within.

However, a Class may be a member of multiple Categories, eg:

```common-lisp
(SZMAClass-addCategories "SZCEPart-PipeRun" (list "Mechanical" "Piping"))
```

where `SZMAClass-addCategories` has the following signature:

`(SZMAClass-addCategories ClassName Categories)`

And:

| Item | Type | Description |
| --------- | --------- | --------- |
| ClassName | String | Name of the Class |
| Categories | List:Category | a list of Categories for the Class |

For the full list - refer to the [Categories](/docs/categories.html) document.


> **Notes:**<br>
> - Each Category has a corresponding **M-** (Make) command that can be entered at the command line.
> - This resolves class naming issues as the class name is now about functionality rather than class access.


## Strings vs Symbols

**SOZ** uses Strings within the code for Arguments, Class, Method and Function names and documentation strings, because:

- converting strings to symbols is easy.
- Users have to be able to read the strings.
- It enables automatic documentation of the system.


## The Meta Environment

The **Meta** Environment exists as a single entity in memory at run-time and stores and indexes all relationships between:

- Classes,
- Functions,
- Methods
- Categories
- Settings

The **Meta** information is accessed to determine things such as:

- Superclass and Subclass information
- Function / Method signatures and their required Types / Classes.

