---
layout: default
description: Sub Repo, with rigging specific functionality included.
type: Private
status: Beta
---

# soz-rigging

## Introduction

This repo provides crane rigging functionality for **soz-live**.

## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [SZOBObject](/classes/SZOBObject.html)
    - [SZOBCAD](/classes/SZOBCAD.html)
      - [AcDbObject](/classes/AcDbObject.html)
        - [AcDbTableRecord](/classes/AcDbTableRecord.html)
          - [AcDbBlock](/classes/AcDbBlock.html)
            - [SZCEModelDef](/classes/SZCEModelDef.html)
              - [SZCERigging-ChainLink](/classes/SZCERigging-ChainLink.html)
                - [SZCERigging-Link](/classes/SZCERigging-Link.html)
              - [SZCERigging-Shackle](/classes/SZCERigging-Shackle.html)
                - [SZCERigging-Shackle-Bow](/classes/SZCERigging-Shackle-Bow.html)
      - [SZCOObject](/classes/SZCOObject.html)
        - [SZCORigging](/classes/SZCORigging.html)
          - [SZCERigging](/classes/SZCERigging.html)
            - [SZCERigging-Arrgt](/classes/SZCERigging-Arrgt.html)
              - [SZCERigging-Arrgt-1xL](/classes/SZCERigging-Arrgt-1xL.html)
              - [SZCERigging-Arrgt-2xL](/classes/SZCERigging-Arrgt-2xL.html)
              - [SZCERigging-Arrgt-2xL-SB-2x1xL](/classes/SZCERigging-Arrgt-2xL-SB-2x1xL.html)
              - [SZCERigging-Arrgt-2xL-SB-2x2xL](/classes/SZCERigging-Arrgt-2xL-SB-2x2xL.html)
              - [SZCERigging-Arrgt-4xL](/classes/SZCERigging-Arrgt-4xL.html)
              - [SZCERigging-Arrgt-OnLine](/classes/SZCERigging-Arrgt-OnLine.html)
          - [SZCORigging-Leg](/classes/SZCORigging-Leg.html)
          - [SZCORigging-Object](/classes/SZCORigging-Object.html)
            - [SZCORigging-Item](/classes/SZCORigging-Item.html)
              - [SZCORigging-Assy](/classes/SZCORigging-Assy.html)
                - [SZCORigging-ChainAssy](/classes/SZCORigging-ChainAssy.html)
              - [SZCORigging-Bar](/classes/SZCORigging-Bar.html)
              - [SZCORigging-Link](/classes/SZCORigging-Link.html)
                - [SZCORigging-WireGrommet](/classes/SZCORigging-WireGrommet.html)
              - [SZCORigging-Shackle](/classes/SZCORigging-Shackle.html)
              - [SZCORigging-Sling](/classes/SZCORigging-Sling.html)
                - [SZCORigging-Chain](/classes/SZCORigging-Chain.html)
                - [SZCORigging-RoundSling](/classes/SZCORigging-RoundSling.html)
    - [SZOBValue](/classes/SZOBValue.html)
      - [SZGEObject](/classes/SZGEObject.html)
        - [SZGECurve](/classes/SZGECurve.html)
          - [SZGE2dCurve](/classes/SZGE2dCurve.html)
            - [SZGELoop](/classes/SZGELoop.html)
              - [SZGEShape](/classes/SZGEShape.html)
                - [SZGEShape-Shackle-Eye](/classes/SZGEShape-Shackle-Eye.html)

Version:  1.26.4
<br>
Date: 20251031.1809
