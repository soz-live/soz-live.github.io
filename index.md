---
layout: default
---

# Home

## Contents

- Home
  - [Introduction](#introduction)
  - [Status](#status)
  - [Platforms](#platforms)  
  - [SOZ](#soz)
    - [The What of SOZ](#the-what-of-soz)  
    - [The Why of SOZ](#the-why-of-soz)  
  - [LIVE](#live)
    - [The What of LIVE](#the-what-of-live)  
    - [The How of LIVE](#the-how-of-live)


## Introduction

**SOZ-LIVE** is a CAD extension, written in Lisp.  

**SOZ-LIVE** is a collection of over 2600 Lisp routines, that enables the creation of complex CAD entities, from a series of inputs of simpler objects.

## Status

The current status of the project is **Private Beta**.

## Platforms

**SOZ-LIVE** can be run within both BricsCAD and AutoCAD.

- 3D Modelling functionality requires BricsCAD Pro or above, or full AutoCAD.
- Some Civil functionality is limited to BricsCAD Pro or above only.


## SOZ

### The What of SOZ

**SOZ** = Scripted ObjectZ  

**SOZ** is a means to combine:

- Functional Programming (FP)
- Object Oriented Programming (OOP) 
- Scripting

using Lisp.
 

### The Why of SOZ

**SOZ** was created to enable:

- powerful but simple access to CAD objects through Lisp.
- parametric modelling of complex 3D Solid entities.

Along the way, benefits of using the **SOZ** approach became apparent, including:

- Reduced code duplication.
- Ease of extending classes.
- Adding to the functionality of CAD.  

## LIVE 

### The What of LIVE

**LIVE** = Lisp Interactive Visual Environment

**LIVE** is a Node-based visual User Interface (UI) written in **SOZ** that enables the user to create visual scripts for iterative design.

### The How of LIVE

The routines are built into the Core of **SOZ**, and consist of under 1000 lines of code.

**LIVE** objects, such as Nodes and Links, are created in PaperSpace while the modelling entities are created in ModelSpace.

