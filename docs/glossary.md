---
layout: default
---
# Glossary

## Contents

- Glossary
  - [Alist](#alist)
  - [API](#api)
  - [Atom](#atom)
  - [CAD](#cad)
  - [Class](#class)
  - [CLI](#cli)
  - [DIP](#dip)
  - [DRY](#dry)
  - [FP](#fp)
  - [Function](#function)
  - [GUI](#gui)
  - [ID](#id)
  - [ISP](#isp)
  - [Lisp](#lisp)
  - [List](#list)
  - [LIVE](#live)
  - [LSP](#lsp)
  - [Method](#method)
  - [Object](#object)
  - [OCP](#ocp)
  - [OOP](#oop)
  - [Runtime](#runtime)
  - [SOLID](#solid)
  - [SOZ](#soz)
  - [SRP](#srp)
  - [String](#string)
  - [Structure](#structure)
  - [Symbol](#symbol)
  - [Type](#type)
  - [UI](#ui)




## Alist

Inside Lisp, a key-value association [list](#list), where the Keys are Atoms and the Values may be Atoms or Lists.  
In other languages they are called dictionaries.  


## API

Application Programming Interface. <br> A means of communicating between different programming languages within an application.


## Atom

An atomic thing. Examples include Numbers, Strings & Symbols.


## CAD

Computer Aided Design: software for representing real world objects in a virtual environment. <br> Most CAD software provide various APIs for manipulating the objects in the model.


## Class

A template for creating objects.<br>
Also known as a Type.


## CLI

Command-Line user Interface		


## DIP

Stands for the Dependency Inversion Priciple and is the D in [SOLID](#solid). <br> It describes the strategy of depending upon Abstractions (abstract classes) and not to depend upon concretions (actual classes).


## DRY

Stands for the Don't Repeat Yourself <br> It describes the programming strategy of defining something once and using it many times. <br>Often used in functions and variables.


## FP

Functional Programming. <br> A programming paradigm based upon processing functions.


## Function

A function is a list of instructions or other functions for the computer to process using a programming language.


## GUI

Graphical User Interface - generally using dialog boxes.


## ID

An Identifier used as the reference pointer to an Object. <br> In SOZ it is a string with a unique format.


## ISP

Stands for the Interface Segregation Principle and is the I in [SOLID](#solid). <br> It describes that many client specific interfaces are better than one general purpose interface.


## Lisp

A programming language based around LISt Processing.  
Provided as one of the [API](#api)s within some [CAD](#cad) software.   


## List

A list of values stored as one thing - opposite of an Atom. <br> Lisp has a number of functions specifically available to utilise this data type.


## LIVE

A node based visual User Interface, written using SOZ, where objects are represented by nodes and links between nodes to display the flow of data.  
With LIVE standing for Lisp Interactive Visual Environment.  


## LSP

Stands for Liskov Substitution Principle and is the L in [SOLID](#solid). <br> It describes the requirement that all sub-types of x must be able to be used anywhere that types of x are required.


## Method

A function defined for a particular Class.


## Object

A self contained thing - interacting with other Objects through methods. <br> An instance of a Class created at run-time. <br> Passed and referenced as an ID.


## OCP

Stands for the Open Closed Principle and is the O in [SOLID](#solid). <br> It describes the requirement that a module should be open for extension but closed for modification.


## OOP

Object Oriented Programming. <br> A programming paradigm based upon working with Objects and Methods.


## Runtime

The time during which the program is being executed.


## SOLID

A set of five governing principles used to define proper programming.  
Each of the letters stand for a different principle.  
Refer to the below glossary entries for the five principles.  


## SOZ

An extension of the [Lisp](#lisp) programming language within [CAD](#cad) that provides a means of doing [OOP](#oop) using a [FP](#fp) language to create and manipulate [objects](#object).  
The name SOZ comes from Scripted ObjectZ, with the Z used to indicate the reflective nature of the language.  


## SRP

Stands for the Single Responsibility Principle and is the S in [SOLID](#solid). <br> It describes the requirement that there should never be more than one reason for a class to change.


## String

A human readable series of characters making words etc..


## Structure

Inside SOZ, a String-Keyed Alist.


## Symbol

A computer readable series of characters used during processing.


## Type

Every Object belongs to a particular type or is a sub-type of something else.<br>
Also know as a Class.


## UI

User Interface - for users to interact with the program. <br> In SOZ there are three UIs - a CLI, a GUI and LIVE.

Date: 20250414.205
