---
layout: default
description: Sub Repo, with rigging specific functionality included.
---

# soz-rigging

## Introduction

This repo provides crane rigging functionality for **soz-live**.

## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [SZOBObject](/classes/SZOBObject.html)
    - [SZGEObject](/classes/SZGEObject.html)
      - [SZGECurve](/classes/SZGECurve.html)
        - [SZGE2dCurve](/classes/SZGE2dCurve.html)
          - [SZGELoop](/classes/SZGELoop.html)
            - [SZGEShape](/classes/SZGEShape.html)
              - [SZGEShape-Shackle-Eye](/classes/SZGEShape-Shackle-Eye.html)
    - [SZOBCAD](/classes/SZOBCAD.html)
      - [AcDbObject](/classes/AcDbObject.html)
        - [AcDbTableRecord](/classes/AcDbTableRecord.html)
          - [AcDbBlock](/classes/AcDbBlock.html)
            - [SZCEModelDef](/classes/SZCEModelDef.html)
              - [SZCEModelDef-ChainLink](/classes/SZCEModelDef-ChainLink.html)
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
            - [SZCORigging-Assy](/classes/SZCORigging-Assy.html)
              - [SZCORigging-Leg](/classes/SZCORigging-Leg.html)
            - [SZCORigging-Item](/classes/SZCORigging-Item.html)
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

Version:  1.22.5
<br>
Date: 20250414.205
