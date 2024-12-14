# Users

## Introduction

This page goes into details for users working with **SOZ-LIVE**.  

## Concepts

The basic concepts required to understand this document are:

- [Class](#class)
- [Object](#object)
- [Entity](#entity)
- [Identifiers](#identifiers)
- [Method](#method)


### Class

Within **SOZ-LIVE** the basic reasoning behind class and object creation is:<br>

**Could it be used again?**<br>

If it could be used again somewhere else then it becomes an Object of a specific class.<br>
A Class is then created to template the creation of each object.


### Object

Within **SOZ-LIVE** an Object is the base level of things created.

They are non-graphical in nature and range from simple values such as:

- a [Real](classes/Real.md) value - a real number
- a [Boolean](classes/Boolean.md) value - ie either True or False.
- a [SZLPReal](classes/SZLPReal.md) value object of a real number.

through to complex geometric objects that utilise other objects and entities in their calculated value(s):

- a [SZGEPoint-AcDbCircle-Center](classes/SZGEPoint-AcDbCircle-Center.md) object - that returns the center [Point](classes/Point.md) of a [AcDbCircle](classes/AcDbCircle.md) Entity.
- a [SZGEPattern2D-Rectangular](classes/SZGEPattern2D-Rectangular.md) object - that creates and returns a list of [TMatrix](classes/TMatrix.md) values for the insertion of Entities into the Model.  


> **Notes:**<br>
> - A [Real](classes/Real.md) value entered into a dialog box is stored as a string until required by the program. 
> - This enables lisp equations such as `(/ 1.0 3.0)` to be entered and calculated to full precision as and when required.


### Entity

Within **SOZ-LIVE** an Entity is derived from Object and describes Objects that are graphical in nature.

Base classes predominantly begin with the prefix `AcDb`, and derived classes are typically prefixed with `SZCE`.



### Identifiers

All objects in **SOZ** are stored and passed by reference to an **ID** - that is a string incorporating the object's Handle.  
eg: **`"#O#AA5"`** would be the **SOZ** object with the handle **AA5**.

> **Notes:**<br>
> - All Make routines return the **ID** of the object / entity that was created.


### Method

Within **SOZ** each function is defined as a Method of a particular Class.  

When interacting with **SOZ** you are basically manipulating Objects by applying a method of an Object.


## SOZ Usage

To use **SOZ-LIVE** follow the next few sections...


### Downloading SOZ

Download the complete project file **SOZ-LIVE.lsp** from the **code** directory and save it into a local directory for loading into CAD.

> **Notes:**<br>
> - While the source code is split into multiple files, the entire project is contained within the one combined Lisp file.  
> - For more information on the code files - refer to the README in that directory.


### Loading SOZ

Load the file in the usual manner into CAD for Lisp routines.

> **Notes:**<br>
> - You can then set it to auto-load in the usual manner.


### SOZ Commands

You can interact with the program in a number of ways.

The easiest way to interact with **SOZ** is to type **Y** on the command line - a dialog box appears with a tree-view of options available to select. <br>

> **Notes:**<br>
> - **Y** is the only key not used as a standard CAD command short-cut.  
> - All **SOZ** commands are in the same format, eg `M-...`, so as not to interfere with conventional CAD shortcuts.  
> - Once you know the name of a command, eg. `M-Circle` to create a Circle or `M-Part` to create a Part, you can just type that command instead.


## SOZ Dialogs

Each **SOZ-LIVE** Class has a dialog box developed on-the-fly, depending on the arguments for the Class.

Each argument to be specified creates another entry in the dialog box to be filled in by the user.

> **Notes:**<br>
> Only fully completed dialogs - one with valid entries for each field, will be parsed by the Make routine properly and return a valid Object.

The entry is either an **atom** field or a **list** field - depending upon the type of each of the arguments for the Class...

For example, the dialog for the class [SZGELine](classes/SZGELine.md) has two required arguments:

- POINT0 - an atom field which is required to be of type [SZGEPoint](classes/SZGEPoint.md)
- POINT1 - an atom field which is required to be of type [SZGEPoint](classes/SZGEPoint.md)

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
<br><br>
> **Notes:**<br>
> - All options are prefixed with "User_" to indicate that they are user methods - able to be selected by the User.


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
- reverse the list
- remove an item
- edit an item
<br>

 > **Tips:**<br>
 > - Double clicking on an Item is the same as Editing the Item.
 

## Process

The basic **SOZ-LIVE** process for drawing develoment follows the following four phases:

1. Specify non-graphical Objects and Values.
2. Draft graphical Entities using Objects and Values.
3. Model Parts and Assemblies using Entities, Objects and Values.
4. Present

During each phase the basic approach to using **SOZ** is followed:

- **Make** objects - using the **Y** or **M-** commands
- **Edit** objects - using the **E-** commands, within a dialog box.
- **Update** objects - this is part of the Edit command.

