---
layout: default
---

# Basics

## Contents

- Basics
  - [Introduction](#introduction)
  - [Class](#class)
  - [Object](#object)
  - [Entity](#entity)
  - [Identifiers](#identifiers)
  - [Methods](#methods)  
  - [Commands](#commands)
  - [Dialog Boxes](#dialog-boxes)
    - [Atom Fields](#atom-fields)
    - [List Fields](#list-fields)    
  - [LIVE](#live)
    - [LIVE Nodes](#live-nodes)
    - [LIVE Links](#live-links)     
    - [LIVE Points](#live-points)    
  - [Drawing Process](#drawing-process)
    - [Specify](#specify)
    - [Draft](#draft)
    - [Model](#Model)
      - [Part](#part)
      - [Feature](#feature)
      - [Assembly](#assembly)    
    - [Present](#present)  
  

  
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

{% include note-content.html content="<br> - Except for Lisp values, each class has a four letter prefix that identifies it as belonging to a particular part of the class hierarchy.<br> - Refer to the Prefixes document for details." %}


## Object

An Object is the base level of things created.

They are non-graphical in nature and range from simple values such as:

- [Real](/classes/Real.html) - a Lisp real number
- [Boolean](/classes/Boolean.html) - a value that is either True or False.

Through to complex geometric objects that utilise other objects and entities in their calculated value(s):

- [SZGEPoint-AcDbCircle-Center](/classes/SZGEPoint-AcDbCircle-Center.html) object - that returns the center [Point](/classes/Point.html) of a [AcDbCircle](/classes/AcDbCircle.html) Entity.
- [SZGEPattern2D-Rectangular](/classes/SZGEPattern2D-Rectangular.html) object - that creates and returns a list of [TMatrix](/classes/TMatrix.html) values for the insertion of Entities into the Model in a Rectangular 2D Pattern.  


{% include note-content.html content="<br> - A Real value entered into a dialog box is stored as a string until required by the program.<br> - This enables lisp equations such as (/ 1.0 3.0) to be entered and calculated to full precision as and when required." %}

## Entity

An Entity is a type of Object that are graphical in nature.

Base entity classes predominantly begin with the prefix `AcDb`, and derived classes are typically prefixed with `SZCE`.


## Identifiers

All objects in **SOZ** are stored and passed by reference to an **ID** - that is a string incorporating the object's Handle.  
eg: **`"#O#AA5"`** would be the **SOZ** object with the handle **AA5**.

{% include note-content.html content="<br> - All Make routines return the ID of the object / entity that was created." %}

## Methods

Within **SOZ** each function is defined as a Method of a particular Class.  

When interacting with **SOZ** you are basically manipulating Objects by applying a method to the Object.


## Commands

You can interact with the program in a number of ways.

The easiest way to interact with **SOZ** is to type **Y** on the command line - a dialog box appears with a tree-view of options to select from.<br>

The full hierarchial list of of commands is [here](/docs/commands.html).

{% include note-content.html content="<br> - All SOZ commands are in the same format, eg M-... so as not to interfere with conventional CAD shortcuts.<br> - Once you know the name of a command, you can type that command instead.<br> - Y was chosen as it is the only key not used as a standard CAD command shortcut." %}


## Dialog Boxes

Each **SOZ-LIVE** Class and Function has a dialog box developed on-the-fly, depending on the arguments for the Class or Function.

Each argument to be specified creates another entry in the dialog box to be filled in by the user.

{% include note-content.html content="<br> - Only fully completed dialogs - one with valid entries for each field, will be parsed by the Make routine properly and return a valid Object." %}

The entry is either an **atom** field or a **list** field - depending upon the type of each of the arguments for the Class...

For example, the dialog for the class [SZGELine](/classes/SZGELine.html) has two required arguments:

- POINT0 - an atom field which is required to be of type [SZGEPoint](/classes/SZGEPoint.html)
- POINT1 - an atom field which is required to be of type [SZGEPoint](/classes/SZGEPoint.html)


{% include note-content.html content="<br> - Any class that is derived or one that interfaces with the type is also valid.<br> - The alternative classes available for each dialog are available from the ... button at the top of the dialog next to the Class Name.<br> - You can Cut and Paste values from one field to another - as long as the Type of the Value / Object / Entity is compatible." %}

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

{% include note-content.html content="<br> - All options are prefixed with User_ to indicate that they are user methods - selectable by the User." %}

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

{% include note-content.html content="<br> - Double clicking on an Item Edits the Item." %}

 
## LIVE

**LIVE** is a Node-Based UI for **SOZ** that enables the user to create visual scripts for iterative design.

The routines are built into the Core of **SOZ**, and consist of under 1000 lines of code.

Functionality includes:

- Adding Nodes,
- Adding Links between the Nodes
- Editing Nodes
- Updating Nodes and Entities.
- Deleting Nodes and Links

**LIVE** objects are created in PaperSpace while the modelling entities are created in ModelSpace.

The three Object Types for **LIVE** are:

- Nodes
- Links
- Points


### LIVE Nodes

A Node is the graphical object that represents data that can be edited and updated to visualise alternative designs.

In **LIVE**, a Node is a BlockReference Entity, an instance of a Block Object that represents the Function / Method being visualised.

In **SOZ-LIVE** any Method, including all Make methods for Classes can be used as Nodes, thereby giving the greatest flexibility to the system possible.

Every Method has 0 or more inputs and a Return value. These are shown as Attributes within the Block.


### LIVE Links

A Link is the graphical object that represents the flow of data from one Node to another. (Typically Left to Right.)

In **LIVE**, a Link is a 3dPolyline Entity that is drawn from a Point to a Point.

Each Link will update when the corresponding Node is moved or edited.


### LIVE Points

A Point is the graphical object that enables picking of data Values within a Node.

In **LIVE**, a Point is a Point Entity that is drawn at each of the Values of the Node - both Inputs and Return values.

Each Point will update when the corresponding Node is moved or edited.


## Drawing Process

The basic **SOZ-LIVE** process for drawing develoment follows four phases:

- [Specify](#specify)
- [Draft](#draft)
- [Model](#Model)
- [Present](#present)

During each phase the basic approach to using **SOZ** is followed:

- **Make** objects & entities 
  - using the **Y** command or **M-\*** commands listed [here](/docs/commands.html).
- **Edit** objects & entities 
  - using the **E-\*** commands.
- **Update** the model 
  - this is done from within the **Edit** commands.


### Specify

The Objects and Values that form the basis for the Entities are created in this phase.  
These inclde the likes of:

- Numbers
- Equations
- Calculations
- Geometric Values and Objects:
  - Shapes
  - Profiles
  - Curves
  - Points
  - etc.


### Draft

The Entities that form the basis for the Models are created in this phase:

 - Points
 - Planes
 - Curves
  - Lines
  - Arcs
  - Circles
  - etc
- Grids
- etc.  

### Model

Modelling Entities are created in the phase, using previously defined Entities and objects:

- [Part](#part)
- [Feature](#feature)
- [Assembly](#assembly)

#### Part

Parts are made of Features.

#### Feature

There are a variety of types of Features that can be created. Including

- Boolean Solids
  - Union
  - Intersection
  - Subtraction
- Corners
  - Chamfers
  - Fillets
- Slicing to Planes
- Profile Cuts
- Boolean Toolbodies

#### Assembly

Assemblies are made of Parts.


### Present

Currently the presentation of the model is out of the scope of **SOZ-LIVE**

