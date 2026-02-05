---
layout: default
---

# Technical

## Contents

- Technical
  - [Introduction](#introduction)
  - [Class](#class)
  - [Object](#object)
  - [Entity](#entity)
  - [Identifiers](#identifiers)
  - [Methods](#methods)  
  

  
## Introduction

This page contains technical concepts for users working with **SOZ-LIVE**.


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

{% include note-icon.html %}  
> Except for Lisp values, each class has a four letter prefix that identifies it as belonging to a particular part of the class hierarchy.  
> Refer to the [Prefixes](/docs/prefixes.html) document for details.


## Object

An Object is the base level of things created.

They are non-graphical in nature and range from simple values such as:

- [Real](/classes/Real.html) - a Lisp real number
- [Boolean](/classes/Boolean.html) - a value that is either True or False.

Through to complex geometric objects that utilise other objects and entities in their calculated value(s):

- [SZGEPoint-AcDbCircle-Center](/classes/SZGEPoint-AcDbCircle-Center.html) object - that returns the center [Point](/classes/Point.html) of a [AcDbCircle](/classes/AcDbCircle.html) Entity.
- [SZGEPattern2D-Rectangular](/classes/SZGEPattern2D-Rectangular.html) object - that creates and returns a list of [TMatrix](/classes/TMatrix.html) values for the insertion of Entities into the Model in a Rectangular 2D Pattern.  

{% include note-icon.html %}  
> A Real value entered into a dialog box is stored as a string until required by the program.

## Entity

An Entity is a type of Object that are graphical in nature.

Base entity classes predominantly begin with the prefix `AcDb`, and derived classes are typically prefixed with `SZCE`.


## Identifiers

All objects in **SOZ** are stored and passed by reference to an **ID** - that is a string incorporating the object's Handle.  
eg: **`"#O#AA5"`** would be the **SOZ** object with the handle **AA5**.

{% include note-icon.html %}  
> All Make routines return the ID of the object / entity that was created.  

## Methods

Within **SOZ** each function is defined as a Method of a particular Class.  

When interacting with **SOZ** you are basically manipulating Objects by applying a method to the Object.


