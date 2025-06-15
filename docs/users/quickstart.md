---
layout: default
---

# Quickstart Guide

## Contents

- Quickstart Guide
  - [Introduction](#introduction)
  - [Downloading SOZ](#downloading-soz)
  - [Loading SOZ](#loading-soz)
  - [SOZ Commands](#soz-commands)
  - [Process](#process)
  

## Introduction

To use **SOZ-LIVE** follow the sections in this Guide...


## Downloading SOZ

Download the complete project file **SOZ-LIVE.lsp** from the **code** directory in the repo, and save it into a local directory for loading into CAD.

> **Notes:**<br>
> - While the source code is split into multiple files, the entire project is contained within the one combined Lisp file.  
> - For more information on the code files - refer to the README in repo's code directory.


## Loading SOZ

Load the file `soz-live.lsp` into CAD using the standard "Appload" command.  
It will load the other repo files as required in the sequence specified within the file.  

> **Notes:**<br>
> - You can set it to auto-load for each drawing, if you plan to use it regularly.


## SOZ Commands

You can interact with the program in a number of ways.

The easiest way to interact with **SOZ** is to type **Y** on the command line - a dialog box appears with a tree-view of options available to select.<br>

> **Notes:**<br>
> - All **SOZ** commands are in the same format, eg `M-...`, so as not to interfere with conventional CAD shortcuts.  
> - Once you know the name of a command, eg. `M-Circle` to create a Circle or `M-Part` to create a Part, you can just type that command instead.  
> - **Y** was chosen as the shortcut as it is the only key not used as a standard CAD command shortcut.  


## Process

The basic **SOZ-LIVE** process for drawing develoment follows four phases:

1. **Specify** - non-graphical Objects and Values.
2. **Draft** - graphical Entities using Objects and Values.
3. **Model** - Parts and Assemblies using Entities, Objects and Values.
4. **Present** - Entities into a final layout.

During each phase the basic approach to using **SOZ** is followed:

- **Make** objects & entities - using the **Y** or **M-** commands
- **Edit** objects & entities - using the **E-** commands, within a dialog box.
- **Update** the objects & entities - this is done during the **Edit** commands.

