---
layout: default
---

# Basic Concepts

## Contents

- Basic Concepts
  - [Introduction](#introduction)
  - [Class](#class)
  - [Object](#object)
  - [Entity](#entity)
  - [Identifiers](#identifiers)
  - [Methods](#methods)  
    

## Introduction

This page contains basic concepts for users working with **SOZ-LIVE**.  


## Class

A Class is a template for the creation of an Object.  
Everything that is created in CAD, and in SOZ, is an Object of a particular Class.  
This includes graphical entities such as:

- [AcDbLine](/classes/AcDbLine.html) - a 3d Line entity - between two points.
- [SZCEPart](/classes/SZCEPart.html) - a complex derived entity containing Features, to define a parametric 3d Enitity.  

<br>
Through to non-graphical objects such as:

- [SZLPReal](/classes/SZLPReal.html) - a value object for a real number.
- [SZLPReals](/classes/SZLPReals.html) - a value object for a list of Real Numbers.

{% include note.html content="<br>- Except for Lisp values, each class has a four letter prefix that identifies it as belonging to a particular part of the class hierarchy.<br>- Refer to the Prefixes document for details." %}


## Object

Within **SOZ-LIVE** an Object is the base level of things created.

They are non-graphical in nature and range from simple values such as:

- [Real](/classes/Real.html) - a Lisp real number
- [Boolean](/classes/Boolean.html) - a value that is either True or False.

Through to complex geometric objects that utilise other objects and entities in their calculated value(s):

- [SZGEPoint-AcDbCircle-Center](/classes/SZGEPoint-AcDbCircle-Center.html) object - that returns the center [Point](/classes/Point.html) of a [AcDbCircle](/classes/AcDbCircle.html) Entity.
- [SZGEPattern2D-Rectangular](/classes/SZGEPattern2D-Rectangular.html) object - that creates and returns a list of [TMatrix](/classes/TMatrix.html) values for the insertion of Entities into the Model in a Rectangular 2D Pattern.  


{% include note.html content="<br>- A Real value entered into a dialog box is stored as a string until required by the program.<br>- This enables lisp equations such as (/ 1.0 3.0) to be entered and calculated to full precision as and when required." %}

## Entity

Within **SOZ-LIVE** an Entity is derived from Object and describes Objects that are graphical in nature.

Base entity classes predominantly begin with the prefix `AcDb`, and derived classes are typically prefixed with `SZCE`.


## Identifiers

All objects in **SOZ** are stored and passed by reference to an **ID** - that is a string incorporating the object's Handle.  
eg: **`"#O#AA5"`** would be the **SOZ** object with the handle **AA5**.

{% include note.html content="<br>- All Make routines return the ID of the object / entity that was created." %}

## Method

Within **SOZ** each function is defined as a Method of a particular Class.  

When interacting with **SOZ** you are basically manipulating Objects by applying a method to the Object.

