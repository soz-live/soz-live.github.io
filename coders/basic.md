---
layout: default
---

# Basics

## Contents

- Basics
  - [Introduction](#introduction)
  - [Lisp Introduction](#lisp-introduction)
    - [Lisp Background](#lisp-background)
    - [AutoLISP Limitations](#autolisp-limitations)
    - [AutoLISP Development](#autolisp-development)
    - [AutoLISP Future](#autolisp-future)
  - [Lisp Basics](#lisp-basics)
    - [Lisp Functions](#lisp-functions)
    - [Function Renaming](#function-renaming)  
  - [Strings vs Symbols](#strings-vs-symbols)
  - [The Meta Environment](#the-meta-environment)
  - [Types](#types)  
  - [Classes](#classes)
  - [Objects](#objects)
  - [Interfaces](#interfaces)
  - [Categories](#categories) 
  - [Methods](#methods)
    - [Method Naming](#method-naming)
    - [Method Dispatch](#method-dispatch)
    - [Type checking](#type-checking)
    

## Introduction

This page contains basic information for coders working with **SOZ**.  


## Lisp Introduction

Lisp, short for LISt Processing, may be one of the oldest programming languages, but it is also one of the most divisive:  

- You either like the syntax or you don't.
- You either get it's simplicity and expressiveness or you don't.

It is for some of those reasons that Lisp has been pushed to the background, with the likes of C, C++, Java, Python, Ruby and others taking the limelight. Yet, there is still a strong a thriving community of programmers who love and revere the languages that have developed from the original Lisp, including:

- Common Lisp, 
- Scheme, 
- Racket, 
- Clojure.


### Lisp Background

Since early on in the history of AutoCAD, a dialect of Lisp was included as a scripting programming language to enable users to improve productivity through the creation of scripts, routines and commands that enabled users to automate complex, repetitive and tedious tasks.
Because of these abilities, Lisp programming became popular amongst many CAD users and a thriving community of programmers pushed the limits of what the language could do.  
  
As competitors to AutoCAD came into the market, they realised the potential, importance and strengths of including the Lisp application programming interface (API) with their products and providing support for users crossing over to their products. 
Thereby enabling users to bring their collection of routines developed over the years with them and maintain their levels of productivity.


### AutoLISP Limitations

Because of its roots, AutoLISP, and it's associated Dialog Control Language (DCL), suffer from limitations when compared to other dialects of Lisp such as Common Lisp and Scheme.  
Limitations of the language include the lack of an object system, a macro system, defining functions with a variable number of arguments and the ability to create closures.
Despite that, developers continue to work on improving it by providing solutions to shortfalls in functionality. 


### AutoLISP Development

While AutoDesk added an Integrated Development Environment (IDE) and support for ActiveX objects in VisualLisp since AutoCAD 2000, there seems to be little interest to improve the AutoLISP API beyond VisualLisp.  
Bricssys, the developer of BricsCAD, has arguably led the way in this regard, with extensive support for Lisp functionality provided by the program as well as continued development of the API and the release of the BricsCAD Lisp Advanced Development Environment (BLADE) in 2018.  
Not only does BricsCAD support both Lisp and DCL in all versions, it can be used across all platforms (Windows, Mac and Linux).  
Recently AutoCAD improved their support for Lisp and DCL to enable use across Windows, Mac and AutoCAD LT.  



### AutoLISP Future

Lisp has outlasted VBA as an API for CAD applications and even without further development of the core language from AutoCAD, the future of Lisp for CAD looks bright, as other players such as BricsCAD take up the slack and continue to promote, develop and push Lisp forward.


## Lisp Basics

Lisp, short for LISt Processing is one of the oldest programming languages.<br>
While it is primarily considered to be a functional language, it has been extended to be whatever is required, including an Object Oriented (OO) language.


### Lisp Functions

To a programmer starting out in Lisp it takes a while to get used to the syntax and naming conventions used within the language. Where:

- `length` - returns the length of a list.
- `strlen` - returns the length of a string.

Part of the problem is that the brevity of function naming is getting in the way of understanding of the functions and their actions.


### Function Renaming

Taking cues from Scheme, a Lisp dialect known for its structured approach to function naming, Lisp can be transformed to the point where code becomes easier to read and understand.

- `length` becomes `list-length`
- `strlen` becomes `string-length`

If applied rigorously, as within **SOZ**, reading Lisp code can become easier to understand and also to program. 

Not only that, it also leads to an understanding that Lisp code can be considered to be Object-Oriented code in disguise.  
Code can easily be turned into a more readily recognisable format for Object-Oriented method application:

`(SZOB-Apply object method args)`

In **SOZ**, it doesn't matter which format you use for method invocation, however to remain in the spirit of Lisp, many Apply calls have been rewritten to the purely functional format:

`(defun SZOB-length (o) (SZOB-Apply o "length" nil))`

Which then enables the function to be used normally within lisp to do things such as find the sum of all lengths of lines within a list, in just one line of code:

`(apply '+ (mapcar 'SZOB-length line-lst))`



## Strings vs Symbols

**SOZ** uses Strings, instead of Symbols, within the code for Arguments, Class, Method and Function names and documentation strings, because:

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


## Types

In **SOZ**, a Type is just another name for a Class.  

There are three main distinctions between types:

- Values - which return a Value as their result
- Objects - which return an **ID** of an object as their result.
- Scripts - which just are run for their internal results.

<br>**SZOBBase** is the base type for all of **SOZ-LIVE**.  

The Base hierarchy of Types for the Project is:

- [SZOBBase](/classes/SZOBBase.html) - Abstract Base class.
  - [Lisp](/classes/Lisp.html) - Abstract Lisp Value Class
  - [SZOBObject](/classes/SZOBObject.html) - Abstract Object Class
  - [SZOBScript](/classes/SZOBScript.html) - Abstract Script Class

The full hierarchy of **SOZ-LIVE** is listed [here](/repos/soz-live.html).  
Each entry is a link to the documentation for the particular class.  


## Classes

All classes are derived from the Base Class - **SZOBBase**.

While **SOZ** only uses single inheritance:

- Classes can share an interface with other classes.
- Classes can be contained in multiple Categories.


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

> {% include note-icon.html %}  
> Many of the specified classes are Abstract classes - meaning that they can't be instanced / objects created from them.  
> They are used to set out the hierarchy in a logical fashion so that LSP works for each type / class specified.



## Objects

All Objects are made using the Make method of the Class, as shown below:

```common-lisp
(SZMAMethod-make "SZGELine" "Make" (list "POINT0" "POINT1") (list "SZGEPoint" "SZGEPoint") "SZGELine" "Make a Line")
(defun SZGELine-make ( POINT0 POINT1 ) (SZOBObject-Maker "SZGELine" )) 
```

This differs to other Lisp OO implementations where a make routine for a **Line** class would be named **make-line**.

The Make arguments are stored on the Object or Entity in an Alist, together with the Class of the Object.
They contain all the information required to Make, Edit and Update the object as and if required.


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

A Category is an orthogonal concept to a Class.

Both have a hierarchy, and both only allow single inheritance within.

However, a Class may be a member of multiple Categories, eg:

```common-lisp
(SZMAClass-addCategories "Name" "SZCEPart-PipeRun" (list "Mechanical" "Piping"))
```

where `SZMAClass-addCategories` has the following signature:

`(SZMAClass-addCategories Type ClassName Categories)`

And:

| Item | Type | Description |
| --------- | --------- | --------- |
| Type | String | The type of the category |
| ClassName | String | Name of the Class |
| Categories | List:Category | a list of Category Names for the Class |

For the full list - refer to the [Categories document](/docs/categories.html).


> {% include note-icon.html %}  
> Each Category has a corresponding M- (Make) command that can be entered at the command line. 
> This resolves class naming issues as the class name can be all about functionality.


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

