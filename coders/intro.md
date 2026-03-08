---
layout: default
---

# Introduction

## Contents

- Introduction
  - [Features](#features)
    - [Structure](#structure)
    - [Object Protocol](#object-protocol)
    - [GUI](#gui)
    - [LIVE](#live)
    - [Documentation](#documentation)
  - [Documents](#documents)


## Features

For coders, **SOZ-LIVE** is a platform for developing additional functionality for CAD, with the following features built in:

- [Structure](#structure)
- [Object Protocol](#object-protocol)
- [GUI](#gui)
- [LIVE](#live)
- [Documentation](#documentation)

It enables coders to use Object Oriented programming (OOP) techniques from within a Functional / Scripting language, Lisp.  


### Structure

The structured approach to coding promotes:

- Consistency
- Readability
- Modularity
- Useability
- Extensibility


Consistency comes from the rigid function naming structure applied in **SOZ**. This has a flow on effect to the rest of the areas and features.
By using a consistent naming structure leads to improved code readability, modularity, useability, extensibility and design simplicity.
It also forms the basis for the Object Protocol, GUI, LIVE and documentation of the system.

Code Readability is important, as it is the coder that has to read and comprehend the code, for debugging and extending etc., prior to it being lodaed into the CAD system for running. **SOZ**'s use of structure and consistency in function naming assists the coder to read what has come before.

Modularity enables use, re-use and extensibility of code. This is enhanced in **SOZ** through the use of Class Prefixes and a layered structure of classes and functions.

Useability of code is improved in **SOZ** though the other facets of the structured approach to coding, while extensibility is enhanced through modularity, consistency and useability.


### Object Protocol

The use of a Meta Environment enables **SOZ**'s object protocol and the ability for **SOZ** to run OOP code inside of Lisp.
The additional calls to register Classes, Categories, Methods, Functions, Interfaces etc. in the Meta Environemnt has a flow on effect as it enables the GUI and LIVE to function as well.
 

### GUI

A fully functional GUI, that is built on the fly for each Class, Arguments, Functions, Methods etc., is an integral part of **SOZ**. All running from the data within the Meta Environment, it enables complete access to the power of **SOZ** from within a Dialog box driven interface, with the ability for the user to choose a variety of methods for each action, from selecting a previously created Object, to picking one from the model, or a LIVE Node, or creating one at the command line (Prompt).


### LIVE

As with the GUI, the built in Node-based UI, **LIVE**, also runs from the same data within the Meta Environment. Basically any function within **SOZ** can be used as a Node within **LIVE**, meaning that it does truly become a Lisp Interactive Visual Environment.


### Documentation

The generation of class, command, category, release and repo documentation is done automatically when creating a new release of the project.
This is all from the data stored within the Meta Environment and as written into the code.
The GitHub Pages site for the project is then updated to reflect the changes.


## Documents

- [Lisp Information](/coders/lisp.html).
- [Basic Information](/coders/basic.html).

