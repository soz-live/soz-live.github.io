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
          - [SZCERigging-Entity](/classes/SZCERigging-Entity.html)
          - [SZCORigging-Arrgt](/classes/SZCORigging-Arrgt.html)
            - [SZCORigging-Arrgt-1xL](/classes/SZCORigging-Arrgt-1xL.html)
            - [SZCORigging-Arrgt-2xL](/classes/SZCORigging-Arrgt-2xL.html)
            - [SZCORigging-Arrgt-2xL-SB-2x1xL](/classes/SZCORigging-Arrgt-2xL-SB-2x1xL.html)
            - [SZCORigging-Arrgt-2xL-SB-2x2xL](/classes/SZCORigging-Arrgt-2xL-SB-2x2xL.html)
            - [SZCORigging-Arrgt-4xL](/classes/SZCORigging-Arrgt-4xL.html)
          - [SZCORigging-Object](/classes/SZCORigging-Object.html)
            - [SZCORigging-Item](/classes/SZCORigging-Item.html)
              - [SZCORigging-Assy](/classes/SZCORigging-Assy.html)
                - [SZCORigging-ChainAssy](/classes/SZCORigging-ChainAssy.html)
              - [SZCORigging-Bar](/classes/SZCORigging-Bar.html)
                - [SZCORigging-LiftingBeam](/classes/SZCORigging-LiftingBeam.html)
                  - [SZCORigging-Triangle](/classes/SZCORigging-Triangle.html)
                - [SZCORigging-SpreaderBar](/classes/SZCORigging-SpreaderBar.html)
              - [SZCORigging-Link](/classes/SZCORigging-Link.html)
                - [SZCORigging-WireGrommet](/classes/SZCORigging-WireGrommet.html)
              - [SZCORigging-Shackle](/classes/SZCORigging-Shackle.html)
              - [SZCORigging-Sling](/classes/SZCORigging-Sling.html)
                - [SZCORigging-Chain](/classes/SZCORigging-Chain.html)
                - [SZCORigging-RoundSling](/classes/SZCORigging-RoundSling.html)
            - [SZCORigging-Leg](/classes/SZCORigging-Leg.html)
    - [SZOBValue](/classes/SZOBValue.html)
      - [SZGEObject](/classes/SZGEObject.html)
        - [SZGECurve](/classes/SZGECurve.html)
          - [SZGE2dCurve](/classes/SZGE2dCurve.html)
            - [SZGELoop](/classes/SZGELoop.html)
              - [SZGEShape](/classes/SZGEShape.html)
                - [SZGEShape-Shackle-Eye](/classes/SZGEShape-Shackle-Eye.html)

Version:  1.26.3
<br>
Date: 20251026.1955
