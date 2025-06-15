---
layout: default
---

# User Basics

## Contents

- User Basics
  - [Introduction](#introduction)
  - [Concepts](#concepts)
    - [Class](#class)
    - [Object](#object)
    - [Entity](#entity)
    - [Identifiers](#identifiers)
    - [Methods](#methods)  
  - [SOZ Dialogs](#soz-dialogs)
    - [Atom Fields](#atom-fields)
    - [List Fields](#list-fields)    
 
    

## Introduction

This page contains basic information for users working with **SOZ-LIVE**.  

## Concepts

The basic concepts required to understand **SOZ-LIVE** are:

- [Class](#class)
- [Object](#object)
- [Entity](#entity)
- [Identifiers](#identifiers)
- [Method](#method)


### Class

A Class is a template for the creation of an Object.  
Everything that is created in CAD, and in SOZ, is an Object of a particular Class.  
This includes graphical entities such as:

- [AcDbLine](/classes/AcDbLine.html) - a 3d Line entity - between two points.
- [SZCEPart](/classes/SZCEPart.html) - a complex derived entity containing Features, to define a parametric 3d Enitity.  

<br>
Through to non-graphical objects such as:

- [SZLPReal](/classes/SZLPReal.html) a value object for a real number.
- [SZLPReals](/classes/SZLPReals.html) avalue object for a list of Real Numbers.


> **Notes:**<br>
> - Except for Lisp values, each class has a 4 letter prefix that identifies it as belonging to a particular part of the class hierarchy.  
> - Refer to the [Prefixes](/docs/prefixes.html) document for details.


### Object

Within **SOZ-LIVE** an Object is the base level of things created.

They are non-graphical in nature and range from simple values such as:

- [Real](/classes/Real.html) - a real number
- [Boolean](/classes/Boolean.html) value - either True or False.

Through to complex geometric objects that utilise other objects and entities in their calculated value(s):

- [SZGEPoint-AcDbCircle-Center](/classes/SZGEPoint-AcDbCircle-Center.html) object - that returns the center [Point](/classes/Point.html) of a [AcDbCircle](/classes/AcDbCircle.html) Entity.
- [SZGEPattern2D-Rectangular](/classes/SZGEPattern2D-Rectangular.html) object - that creates and returns a list of [TMatrix](/classes/TMatrix.html) values for the insertion of Entities into the Model in a Rectangular 2D Pattern.  


> **Notes:**<br>
> - A [Real](/classes/Real.html) value entered into a dialog box is stored as a string until required by the program. 
> - This enables lisp equations such as `(/ 1.0 3.0)` to be entered and calculated to full precision as and when required.


### Entity

Within **SOZ-LIVE** an Entity is derived from Object and describes Objects that are graphical in nature.

Base entity classes predominantly begin with the prefix `AcDb`, and derived classes are typically prefixed with `SZCE`.


### Identifiers

All objects in **SOZ** are stored and passed by reference to an **ID** - that is a string incorporating the object's Handle.  
eg: **`"#O#AA5"`** would be the **SOZ** object with the handle **AA5**.

> **Notes:**<br>
> - All Make routines return the **ID** of the object / entity that was created.


### Method

Within **SOZ** each function is defined as a Method of a particular Class.  

When interacting with **SOZ** you are basically manipulating Objects by applying a method to the Object.


## SOZ Dialogs

Each **SOZ-LIVE** Class has a dialog box developed on-the-fly, depending on the arguments for the Class.

Each argument to be specified creates another entry in the dialog box to be filled in by the user.

> **Notes:**<br>
> Only fully completed dialogs - one with valid entries for each field, will be parsed by the Make routine properly and return a valid Object.

The entry is either an **atom** field or a **list** field - depending upon the type of each of the arguments for the Class...

For example, the dialog for the class [SZGELine](/classes/SZGELine.html) has two required arguments:

- POINT0 - an atom field which is required to be of type [SZGEPoint](/classes/SZGEPoint.html)
- POINT1 - an atom field which is required to be of type [SZGEPoint](/classes/SZGEPoint.html)

> **Notes:**<br>
> - Any class that is derived or one that interfaces with the type is also valid. The alternative classes available for each dialog are available from the `...` button at the top of the dialog next to the Class Name.

> **Tips:**<br>
> - You can Cut and Paste values from one field to another - as long as the Type of the Value / Object / Entity is compatible.


### Atom Fields

Each atom field has a number of components to it..

1. the Border - that contains the name of the class that is required to be specified. eg. SZGEPoint
2. the Key - the name of the argument being specified. eg: POINT0
3. the EditBox - where the value of the argument is entered / displayed
4. the `...` Button - to specify a different class than the one listed in the border. (optional)
5. the Options DropDown - a list of options available to specify the value for the argument.

<br>
Where the Options vary depending upon the Class being created, but include:

- Make - Which brings up a new dialog box to create an object of the specific Class
- Select - Which brings up a new dialog box to select an object of the specific Class.
- Pick - Enables the User to select an Object on the Screen
- Edit - Edits an existing object in a new dialog box.
- Prompt - Use the Command Line version for entering the Class.
<br>
> **Notes:**<br>
> - All options are prefixed with "User_" to indicate that they are user methods - selectable by the User.


### List Fields

Each list field has five components to it..

1. the Border - that contains the name of the class that is required to be specified.
2. the Key - the name of the argument being specified. eg: IOBJS
3. the Make Options Dropdown - at the top of the ListBox.
4. the ListBox - where the values of the argument is displayed - double clicking on a entry will Edit the value.
5. the Edit Options DropDown - a list of options available to Edit the list.

<br>
Where Make Options include:

- Make - Which brings up a new dialog box to create an object of the specific Class.
- Select - Which brings up a new dialog box to select an object of the specific Class.
- Pick - Enables the User to select an Object on the Screen.
- PickSet - Enables the User to select a set of Objects on the Screen.
- PickList - Enables the User to pick a List of Objects on the Screen.

<br>
And Edit Options include:

- Delete the List
- Move Item to first / last / up / down.
- Reverse the list
- Remove an item
- Edit an item
<br>

 > **Tips:**<br>
 > - Double clicking on an Item Edits the Item.
 
