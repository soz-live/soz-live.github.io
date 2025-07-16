---
layout: default
description: Sub Repo, with Developer specific functionality included.
---

# soz-devs

## Introduction

This repo includes functionality for Developers of **soz-live**, including:

- Source code release creation functions and commands
- Scripting routines for Github and PowerShell
- Code Visualisation tools using mapping functions
- Code Documentation tools used during the release of code.


## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [SZOBObject](/classes/SZOBObject.html)
    - [SZDOObject](/classes/SZDOObject.html)
      - [SZDODoc](/classes/SZDODoc.html)
        - [SZDODoc-Block](/classes/SZDODoc-Block.html)
          - [SZDODoc-Block-Header](/classes/SZDODoc-Block-Header.html)
          - [SZDODoc-Block-Single](/classes/SZDODoc-Block-Single.html)
        - [SZDODoc-Document](/classes/SZDODoc-Document.html)
        - [SZDODocs](/classes/SZDODocs.html)
          - [SZDODocs-CSV](/classes/SZDODocs-CSV.html)
      - [SZDOMap](/classes/SZDOMap.html)
        - [SZDOMap-Class](/classes/SZDOMap-Class.html)
        - [SZDOMap-ClassFunc](/classes/SZDOMap-ClassFunc.html)
        - [SZDOMap-ClassFuncLine](/classes/SZDOMap-ClassFuncLine.html)
      - [SZDOObject-IDE](/classes/SZDOObject-IDE.html)
    - [SZOBCAD](/classes/SZOBCAD.html)
      - [AcDbObject](/classes/AcDbObject.html)
        - [AcDbEntity](/classes/AcDbEntity.html)
          - [AcDbAbstractText](/classes/AcDbAbstractText.html)
            - [AcDbText](/classes/AcDbText.html)
              - [SZDOText](/classes/SZDOText.html)
                - [SZDOText-ClassName](/classes/SZDOText-ClassName.html)
                - [SZDOText-FunctionName](/classes/SZDOText-FunctionName.html)
                - [SZDOText-LineOfCode](/classes/SZDOText-LineOfCode.html)
          - [AcDbBlockReference](/classes/AcDbBlockReference.html)
            - [SZDONode](/classes/SZDONode.html)
              - [SZDONode-Function](/classes/SZDONode-Function.html)
          - [AcDbCurve](/classes/AcDbCurve.html)
            - [AcDb3dPolyline](/classes/AcDb3dPolyline.html)
              - [SZDOLink](/classes/SZDOLink.html)
          - [AcDbPoint](/classes/AcDbPoint.html)
            - [SZDOPoint](/classes/SZDOPoint.html)
        - [AcDbTableRecord](/classes/AcDbTableRecord.html)
          - [AcDbBlock](/classes/AcDbBlock.html)
            - [SZDODef](/classes/SZDODef.html)
              - [SZDODef-Function](/classes/SZDODef-Function.html)

Version:  1.25.2
<br>
Date: 20250715.1648
