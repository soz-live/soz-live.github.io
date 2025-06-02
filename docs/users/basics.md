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

- a [Line](/classes/AcDbLine.html) - a 3d Line entity - between two points.
- a [Part](/classes/SZCEPart.html) - a complex derived entity containing Features, to define a parametric 3d Enitity.

through to non-graphical objects such as:

- a [SZLPReal](/classes/SZLPReal.html) value object for a real number.


### Object

Within **SOZ-LIVE** an Object is the base level of things created.

They are non-graphical in nature and range from simple values such as:

- a [Real](/classes/Real.html) value - a real number
- a [Boolean](/classes/Boolean.html) value - ie either True or False.

through to complex geometric objects that utilise other objects and entities in their calculated value(s):

- a [SZGEPoint-AcDbCircle-Center](/classes/SZGEPoint-AcDbCircle-Center.html) object - that returns the center [Point](/classes/Point.html) of a [AcDbCircle](/classes/AcDbCircle.html) Entity.
- a [SZGEPattern2D-Rectangular](/classes/SZGEPattern2D-Rectangular.html) object - that creates and returns a list of [TMatrix](/classes/TMatrix.html) values for the insertion of Entities into the Model.  


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

