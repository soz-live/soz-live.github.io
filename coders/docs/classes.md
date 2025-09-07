---
layout: default
---

# Classes

## Contents

- Classes
  - [Introduction](#introduction)
  - [Types](#types)  
  - [Classes](#classes)
  - [Objects](#objects)
  - [Interfaces](#interfaces)
  - [Categories](#categories)


## Introduction

This page contains basic information for coders on Types and Classes.  


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


{% include note.html content="<br>- Many of the specified classes are Abstract classes - meaning that they can't be instanced / objects created from them.<br>- They are used to set out the hierarchy in a logical fashion so that LSP works for each type / class specified." %}


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

A Category can be considered an orthogonal concept to a Class.

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

{% include note.html content="<br>- Each Category has a corresponding **M-** (Make) command that can be entered at the command line.<br>- This resolves class naming issues as the class name can be all about functionality." %}
