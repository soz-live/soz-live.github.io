---
layout: default
description: Sub Repo with AEC functionality included.
type: Private
status: Beta
---

# soz-aec

## Introduction

This repo includes functionality for:

- Architectural
- Engineering
  - Mechanical
  - Civil
  - Structural
- Construction

workflows.

## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [SZOBObject](/classes/SZOBObject.html)
    - [SZOBCAD](/classes/SZOBCAD.html)
      - [AcDbObject](/classes/AcDbObject.html)
        - [AcDbTableRecord](/classes/AcDbTableRecord.html)
          - [AcDbBlock](/classes/AcDbBlock.html)
            - [SZCEModelDef](/classes/SZCEModelDef.html)
              - [SZCEModel](/classes/SZCEModel.html)
                - [SZCEPart](/classes/SZCEPart.html)
                  - [SZCEPart-Ditch](/classes/SZCEPart-Ditch.html)
                    - [SZCEPart-Ditch-Constant](/classes/SZCEPart-Ditch-Constant.html)
                  - [SZCEPart-Planar](/classes/SZCEPart-Planar.html)
                    - [SZCEPart-Extrusion-AcDbPolyline](/classes/SZCEPart-Extrusion-AcDbPolyline.html)
                      - [SZCEPart-Extrusion-Face](/classes/SZCEPart-Extrusion-Face.html)
      - [SZCOObject](/classes/SZCOObject.html)
        - [SZCEElement](/classes/SZCEElement.html)
          - [SZCECivil](/classes/SZCECivil.html)
          - [SZCEMech](/classes/SZCEMech.html)
        - [SZCOFeature](/classes/SZCOFeature.html)
          - [SZCOFeature-Part](/classes/SZCOFeature-Part.html)
            - [SZCOFeature-3dSolid](/classes/SZCOFeature-3dSolid.html)
              - [SZCOFeature-Extrusion-CutOut](/classes/SZCOFeature-Extrusion-CutOut.html)
      - [SZCOObjects](/classes/SZCOObjects.html)
        - [SZCEEntities](/classes/SZCEEntities.html)
          - [SZCESections](/classes/SZCESections.html)
            - [SZCESections-OnCurve-Chainage-Exported](/classes/SZCESections-OnCurve-Chainage-Exported.html)

Version:  1.27.0
<br>
Date: 20251129.135
