---
layout: default
description: Sub Repo, with Data Import / Export functionality included.
type: Private
status: Beta
---

# soz-files

## Introduction

The **soz-files** repo adds import / export functionality to **SOZ**.

With this repo it is possible to import and export **soz** objects to various file formats.


## SOZ Files - *.DAT

These are **SOZ** objects stored line by line in a file format with the ability to reference preceeding objects using an ID.

They are exported from **SOZ** using the **X-SOZ** command.  

They are imported into **SOZ** using the **I-SOZ** command.

> Note:  
> - As these files only store the arguments for each object they are an extremely compact file format.  
> - While being in text format - they are still easy to read and even edit in a text editor.  


## CSVArray Files - *.CSV

These are **SOZ** objects stored in CSV format with the ability to reference preceeding objects using an ID.

They are exported from **SOZ** using the **X-ARRAY** command.  

And are imported into **SOZ** using the **I-ARRAY** command. 


## Class Files - *.CSV

These are plain CSV files stored in a format for a specific Class, with the name of the class as the filename, eg: SZCEShape-CPurlin.

They are imported into **SOZ** using the **I-CLASS** command.

## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [Lisp](/classes/Lisp.html)
    - [Logical](/classes/Logical.html)
      - [T](/classes/T.html)
        - [Atom](/classes/Atom.html)
          - [File](/classes/File.html)
            - [File-TXT](/classes/File-TXT.html)
              - [File-CSV](/classes/File-CSV.html)
                - [File-CSVArray](/classes/File-CSVArray.html)
              - [File-DAT](/classes/File-DAT.html)
                - [SOZFile](/classes/SOZFile.html)

Version:  1.27.0
<br>
Date: 20251129.135
