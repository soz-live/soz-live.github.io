---
layout: default
---

# Quickstart Guide

## Contents

- Quickstart Guide
  - [Introduction](#introduction)
  - [Downloading SOZ](#downloading-soz)
  - [Loading SOZ](#loading-soz)
  - [Begin Drawing](#begin-drawing)
  

## Introduction

To use **SOZ-LIVE** follow the sections in this Guide...


## Downloading SOZ

Download the complete project file **SOZ-LIVE.lsp** from the **code** directory in the repo, and save it into a local directory for loading into CAD.

{% include note.html content="<br> - While the source code is split into multiple files, the entire project is contained within the one combined Lisp file.<br> - For more information on the code files - refer to the README in repo's code directory." %}

## Loading SOZ

Load the file `soz-live.lsp` into CAD using the standard "Appload" command.  
It will load other repo files as required in the sequence specified within the file.  

{% include note.html content="<br> - You can set it to auto-load for each drawing, if you plan to use it regularly." %}

## Begin Drawing

The basic **SOZ-LIVE** process for drawing develoment follows four phases:

1. **Specify** - non-graphical Objects and Values.
2. **Draft** - graphical Entities using Objects and Values.
3. **Model** - Parts and Assemblies using Entities, Objects and Values.
4. **Present** - Entities into a final layout.

During each phase the basic approach to using **SOZ** is followed:

- **Make** objects & entities 
  - using the **Y** command or **M-\*** commands listed [here](/docs/commands.html).
- **Edit** objects & entities 
  - using the **E-\*** commands.
- **Update** the model 
  - this is done from within the **Edit** commands.


{% include note.html content="<br> - All SOZ commands are in the same format, eg M-... so as not to interfere with conventional CAD shortcuts.<br> - Once you know the name of a command, you can type that command instead.<br> - Y was chosen as it is the only key not used as a standard CAD command shortcut." %}

