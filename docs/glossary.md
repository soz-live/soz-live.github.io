---
layout: default
---

# Glossary

Below is a list of terms and their meanings as used within the project.


## Contents

- 
  - [API](#api)
  - [Alist](#alist)
  - [Atom](#atom)
  - [CAD](#cad)
  - [CLI](#cli)
  - [Class](#class)
  - [DIP](#dip)
  - [DRY](#dry)
  - [FP](#fp)
  - [Function](#function)
  - [GUI](#gui)
  - [ID](#id)
  - [ISP](#isp)
  - [LIVE](#live)
  - [LSP](#lsp)
  - [Lisp](#lisp)
  - [List](#list)
  - [Method](#method)
  - [OCP](#ocp)
  - [OOP](#oop)
  - [Object](#object)
  - [Runtime](#runtime)
  - [SOLID](#solid)
  - [SOZ](#soz)
  - [SRP](#srp)
  - [String](#string)
  - [Structure](#structure)
  - [Symbol](#symbol)
  - [Type](#type)
  - [UI](#ui)




## API

Application Programming Interface. <br> A means of communicating between different programming languages within an application.


## Alist

Inside Lisp, a key-value association list, where the Keys are Atoms and the Values may be Atoms or Lists.


## Atom

An atomic thing. Examples include Numbers, Strings, Symbols.


## CAD

Computer Aided Design software for representing real world objects in a virtual environment. <br> Most CAD software have various APIs for manipulating the objects in the model.


## CLI

Command-Line user Interface		


## Class

A template for creating objects.


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


## LIVE

A node based visual User Interface, written using SOZ, where objects are represented by nodes and links between nodes to display the flow of data.  
With LIVE standing for Lisp Interactive Visual Environment.  


## LSP

Stands for Liskov Substitution Principle and is the L in [SOLID](#solid). <br> It describes the requirement that all sub-types of x must be able to be used anywhere that types of x are required.


## Lisp

A programming language based around LISt Processing.  
Provided as one of the [API](#api)s within some [CAD](#cad) software.   


## List

A list of values stored as one thing - opposite of an Atom. <br> Lisp has a number of functions specifically available to utilise this data type.


## Method

A function defined for a particular Class.


## OCP

Stands for the Open Closed Principle and is the O in [SOLID](#solid). <br> It describes the requirement that a module should be open for extension but closed for modification.


## OOP

Object Oriented Programming. <br> A programming paradigm based upon working with Objects and Methods.


## Object

A self contained thing - interacting with other Objects through methods. <br> An instance of a Class created at run-time. <br> Passed and referenced as an ID.


## Runtime

The time during which the program is being executed.


## SOLID

A set of five governing principles used to define proper programming.  
Each of the letters stand for a different principle.  
Refer to the below glossary entries for the five principles.  


## SOZ

An extension of the [Lisp](#lisp) programming language that provides a means of doing [OOP](#oop) using a [FP](#fp) language to manipulate objects within [CAD](#cad).  
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

Every Object belongs to a particular type or sub-type of something else.<br>AKA a Class.


## UI

User Interface - for users to interact with the program. <br> In SOZ there are three UIs - a CLI, a GUI and LIVE.

Date: 20250301.1406
