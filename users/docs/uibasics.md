---
layout: default
---

# User Interface Basics

## Contents

- User Interface Basics
  - [Introduction](#introduction)
  - [Commands](#commands)
  - [Dialog Boxes](#dialog-boxes)
    - [Atom Fields](#atom-fields)
    - [List Fields](#list-fields)    
  - [LIVE](#live)
    - [LIVE Nodes](#live-nodes)
    - [LIVE Links](#live-links)     
    - [LIVE Points](#live-points)
    

## Introduction

This page contains basic information for users on working with **SOZ-LIVE** user interfaces.  


## Commands

You can interact with the program in a number of ways.

The easiest way to interact with **SOZ** is to type **Y** on the command line - a dialog box appears with a tree-view of options to select from.<br>

The full hierarchial list of of commands is [here](/docs/commands.html).

{% include note.html content="<br>- All SOZ commands are in the same format, eg M-... so as not to interfere with conventional CAD shortcuts.<br>- Once you know the name of a command, you can type that command instead.<br>Y was chosen as it is the only key not used as a standard CAD command shortcut." %}


## Dialog Boxes

Each **SOZ-LIVE** Class and Function has a dialog box developed on-the-fly, depending on the arguments for the Class or Function.

Each argument to be specified creates another entry in the dialog box to be filled in by the user.

{% include note.html content="<br>- Only fully completed dialogs - one with valid entries for each field, will be parsed by the Make routine properly and return a valid Object." %}

The entry is either an **atom** field or a **list** field - depending upon the type of each of the arguments for the Class...

For example, the dialog for the class [SZGELine](/classes/SZGELine.html) has two required arguments:

- POINT0 - an atom field which is required to be of type [SZGEPoint](/classes/SZGEPoint.html)
- POINT1 - an atom field which is required to be of type [SZGEPoint](/classes/SZGEPoint.html)


{% include note.html content="<br>- Any class that is derived or one that interfaces with the type is also valid.<br>- The alternative classes available for each dialog are available from the ... button at the top of the dialog next to the Class Name.<br>- You can Cut and Paste values from one field to another - as long as the Type of the Value / Object / Entity is compatible." %}

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

{% include note.html content="<br>- All options are prefixed with User_ to indicate that they are user methods - selectable by the User." %}

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

{% include note.html content="<br>- Double clicking on an Item Edits the Item." %}

 
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

