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
    - [SZOBCAD](/classes/SZOBCAD.html)
      - [AcDbObject](/classes/AcDbObject.html)
        - [AcDbEntity](/classes/AcDbEntity.html)
          - [AcDbAbstractText](/classes/AcDbAbstractText.html)
            - [AcDbText](/classes/AcDbText.html)
              - [DEVOText](/classes/DEVOText.html)
                - [DEVOText-ClassName](/classes/DEVOText-ClassName.html)
                - [DEVOText-FunctionName](/classes/DEVOText-FunctionName.html)
                - [DEVOText-LineOfCode](/classes/DEVOText-LineOfCode.html)
          - [AcDbBlockReference](/classes/AcDbBlockReference.html)
            - [DEVONode](/classes/DEVONode.html)
              - [DEVONode-Function](/classes/DEVONode-Function.html)
          - [AcDbCurve](/classes/AcDbCurve.html)
            - [AcDb3dPolyline](/classes/AcDb3dPolyline.html)
              - [DEVOLink](/classes/DEVOLink.html)
          - [AcDbPoint](/classes/AcDbPoint.html)
            - [DEVOPoint](/classes/DEVOPoint.html)
        - [AcDbTableRecord](/classes/AcDbTableRecord.html)
          - [AcDbBlock](/classes/AcDbBlock.html)
            - [DEVODef](/classes/DEVODef.html)
              - [DEVODef-Function](/classes/DEVODef-Function.html)
    - [SZOBDevOps](/classes/SZOBDevOps.html)
      - [SZOBDevOps-IDE](/classes/SZOBDevOps-IDE.html)
      - [SZOBDevOps-Map](/classes/SZOBDevOps-Map.html)
        - [SZOBDevOps-Map-Class](/classes/SZOBDevOps-Map-Class.html)
        - [SZOBDevOps-Map-ClassFunc](/classes/SZOBDevOps-Map-ClassFunc.html)
        - [SZOBDevOps-Map-ClassFuncLine](/classes/SZOBDevOps-Map-ClassFuncLine.html)
      - [SZOBDoc](/classes/SZOBDoc.html)
        - [SZOBDoc-Block](/classes/SZOBDoc-Block.html)
          - [SZOBDoc-Block-Header](/classes/SZOBDoc-Block-Header.html)
          - [SZOBDoc-Block-Single](/classes/SZOBDoc-Block-Single.html)
        - [SZOBDoc-Document](/classes/SZOBDoc-Document.html)
        - [SZOBDocs](/classes/SZOBDocs.html)
          - [SZOBDocs-CSV](/classes/SZOBDocs-CSV.html)

Version:  1.24.0
<br>
Date: 20250606.1722
