---
layout: default
description: Sub Repo, with Sling specific functionality included.
type: Private
status: Beta
---

# soz-slings

## Introduction

The **soz-slings** repo adds lifting sling functionality to **SOZ**.

With this repo it is possible to create editable:

- Chains
- Round Slings
- Twisted Chains

## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [SZOBObject](/classes/SZOBObject.html)
    - [SZOBCAD](/classes/SZOBCAD.html)
      - [AcDbObject](/classes/AcDbObject.html)
        - [AcDbGroup](/classes/AcDbGroup.html)
          - [SZCEGroup](/classes/SZCEGroup.html)
            - [SZCEModelGroup](/classes/SZCEModelGroup.html)
              - [SZCEModelGroup-BlockRef](/classes/SZCEModelGroup-BlockRef.html)
                - [SZCEModelGroup-BlockRef-Rotation](/classes/SZCEModelGroup-BlockRef-Rotation.html)
                  - [SZCERigging-Chain](/classes/SZCERigging-Chain.html)
                  - [SZCERigging-TwistedChain](/classes/SZCERigging-TwistedChain.html)
        - [AcDbTableRecord](/classes/AcDbTableRecord.html)
          - [AcDbBlock](/classes/AcDbBlock.html)
            - [SZCEModelDef](/classes/SZCEModelDef.html)
              - [SZCEModel](/classes/SZCEModel.html)
                - [SZCEPart](/classes/SZCEPart.html)
                  - [SZCEPart-FilletedSweep-MultiRadii](/classes/SZCEPart-FilletedSweep-MultiRadii.html)
                    - [SZCERigging-TwistedSling](/classes/SZCERigging-TwistedSling.html)
                - [SZCERigging-TwistedLink](/classes/SZCERigging-TwistedLink.html)
              - [SZCERigging-ChainLink](/classes/SZCERigging-ChainLink.html)
    - [SZOBValue](/classes/SZOBValue.html)
      - [SZGEObject](/classes/SZGEObject.html)
        - [SZGECurve](/classes/SZGECurve.html)
          - [SZGE2dCurve](/classes/SZGE2dCurve.html)
            - [SZGELoop](/classes/SZGELoop.html)
              - [SZGEShape](/classes/SZGEShape.html)
                - [SZGEShape-ChainLink](/classes/SZGEShape-ChainLink.html)
          - [SZGE3dCurve](/classes/SZGE3dCurve.html)
            - [SZGE3dCurve-TwistedSling](/classes/SZGE3dCurve-TwistedSling.html)

Version:  1.26.3
<br>
Date: 20251026.1955
