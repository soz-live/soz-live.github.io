
# Class:	AcDb3dSolid

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [ACISEntity](ACISEntity.html) |
| Subclasses: | [AcDb3dSolid-OnCorridor](AcDb3dSolid-OnCorridor.html) <br> [AcDb3dSolid-BsysTinSurface](AcDb3dSolid-BsysTinSurface.html) <br> [AcDb3dSolid-SZCOSolid](AcDb3dSolid-SZCOSolid.html) <br> [AcDb3dSolid-Loft](AcDb3dSolid-Loft.html) <br> [AcDb3dSolid-Wedge](AcDb3dSolid-Wedge.html) <br> [AcDb3dSolid-Torus](AcDb3dSolid-Torus.html) <br> [AcDb3dSolid-EllipticalCylinder](AcDb3dSolid-EllipticalCylinder.html) <br> [AcDb3dSolid-EllipticalCone](AcDb3dSolid-EllipticalCone.html) <br> [AcDb3dSolid-Cylinder](AcDb3dSolid-Cylinder.html) <br> [AcDb3dSolid-Cone](AcDb3dSolid-Cone.html) <br> [AcDb3dSolid-Box](AcDb3dSolid-Box.html) <br> [AcDb3dSolid-Sphere](AcDb3dSolid-Sphere.html) <br> [AcDb3dSolid-Revolve](AcDb3dSolid-Revolve.html) <br> [AcDb3dSolid-Sweep](AcDb3dSolid-Sweep.html) <br> [AcDb3dSolid-Extrusion-Tapered](AcDb3dSolid-Extrusion-Tapered.html) <br> [AcDb3dSolid-AnySolids](AcDb3dSolid-AnySolids.html) |
| Interfaces: |  |
| Interfaced: | [AcDb3dSolid-AnySolids](AcDb3dSolid-AnySolids.html) |
| Abstract?: | Yes |
| isValue?: | No |
| Help: | AcDb3dSolid Class |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDb3dSolid-Boolean](#AcDb3dSolid-Boolean) <br> [AcDb3dSolid-CubedOnCurve](#AcDb3dSolid-CubedOnCurve) <br> [AcDb3dSolid-DicedOnCurve](#AcDb3dSolid-DicedOnCurve) <br> [AcDb3dSolid-DicedOnWorld](#AcDb3dSolid-DicedOnWorld) <br> [AcDb3dSolid-Section](#AcDb3dSolid-Section) <br> [AcDb3dSolid-SectionPlane](#AcDb3dSolid-SectionPlane) <br> [AcDb3dSolid-SectionTMatrix](#AcDb3dSolid-SectionTMatrix) <br> [AcDb3dSolid-Slice](#AcDb3dSolid-Slice) <br> [AcDb3dSolid-SlicePlane](#AcDb3dSolid-SlicePlane) <br> [AcDb3dSolid-SliceTMatrix](#AcDb3dSolid-SliceTMatrix) <br> [AcDb3dSolid-SlicesOnCurve](#AcDb3dSolid-SlicesOnCurve) <br> [AcDb3dSolid-SlicesOnVector](#AcDb3dSolid-SlicesOnVector) <br> [AcDb3dSolid-Volume](#AcDb3dSolid-Volume) |
| Super: | [ACISEntity-Points](ACISEntity.html) <br> [AcDbEntity-Copy](AcDbEntity.html) <br> [AcDbEntity-Move](AcDbEntity.html) <br> [AcDbEntity-Transformby](AcDbEntity.html) <br> [AcDbEntity-IntersectWith](AcDbEntity.html) <br> [AcDbEntity-Layer](AcDbEntity.html) <br> [AcDbEntity-SZCOColor](AcDbEntity.html) <br> [AcDbEntity-Highlight](AcDbEntity.html) <br> [AcDbEntity-SetVisibility](AcDbEntity.html) <br> [AcDbEntity-Space](AcDbEntity.html) <br> [AcDbEntity-InternalCopy](AcDbEntity.html) <br> [AcDbEntity-ExternalCopy](AcDbEntity.html) <br> [AcDbEntity-SetVisual](AcDbEntity.html) <br> [AcDbEntity-Visual](AcDbEntity.html) <br> [AcDbEntity-User_PickList](AcDbEntity.html) <br> [AcDbEntity-User_Pick](AcDbEntity.html) <br> [AcDbEntity-User_PickModel](AcDbEntity.html) <br> [AcDbEntity-User_PickNode](AcDbEntity.html) <br> [AcDbEntity-User_PickSet](AcDbEntity.html) <br> [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDb3dSolid-Boolean

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| SOLID | [AcDb3dSolid](AcDb3dSolid.html) |  |
| OPERATION | [Enum-AcDbBoolean](Enum-AcDbBoolean.html) |  |
| --- | --- | --- |
| Returns: | [AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Boolean Operation on Solids |

### AcDb3dSolid-CubedOnCurve

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| CURVE | [AcDbCurve](AcDbCurve.html) |  |
| PITCH | [Real](Real.html) |  |
| ACROSS | [Real](Real.html) |  |
| UPWARDS | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Make an AcDb3dSolid |

### AcDb3dSolid-DicedOnCurve

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| CURVE | [AcDbCurve](AcDbCurve.html) |  |
| PITCH | [Real](Real.html) |  |
| DOWN | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Make an AcDb3dSolid |

### AcDb3dSolid-DicedOnWorld

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| XDIST | [Real](Real.html) |  |
| YDIST | [Real](Real.html) |  |
| ZDIST | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Make an AcDb3dSolid |

### AcDb3dSolid-Section

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| POINT1 | [SZGEPoint](SZGEPoint.html) |  |
| POINT2 | [SZGEPoint](SZGEPoint.html) |  |
| POINT3 | [SZGEPoint](SZGEPoint.html) |  |
| --- | --- | --- |
| Returns: | [AcDbRegion](AcDbRegion.html) |
| Help: | Section of a Solid |

### AcDb3dSolid-SectionPlane

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| PLANE | [SZGEPlane](SZGEPlane.html) |  |
| --- | --- | --- |
| Returns: | [AcDbRegion](AcDbRegion.html) |
| Help: | Section of a Solid using a Plane |

### AcDb3dSolid-SectionTMatrix

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| TMATRIX | [SZGETMatrix](SZGETMatrix.html) |  |
| --- | --- | --- |
| Returns: | [AcDbRegion](AcDbRegion.html) |
| Help: | Section of a Solid using a TMatrix |

### AcDb3dSolid-Slice

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| POINT1 | [SZGEPoint](SZGEPoint.html) |  |
| POINT2 | [SZGEPoint](SZGEPoint.html) |  |
| POINT3 | [SZGEPoint](SZGEPoint.html) |  |
| KEEP | [Enum-AcDb3dSolidSlice](Enum-AcDb3dSolidSlice.html) |  |
| --- | --- | --- |
| Returns: | [AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Slice an AcDb3dSolid |

### AcDb3dSolid-SlicePlane

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| PLANE | [SZGEPlane](SZGEPlane.html) |  |
| OFFSET | [Real](Real.html) |  |
| KEEP | [Enum-AcDb3dSolidSlice](Enum-AcDb3dSolidSlice.html) |  |
| --- | --- | --- |
| Returns: | [AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Slice an AcDb3dSolid |

### AcDb3dSolid-SliceTMatrix

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| TMATRIX | [SZGETMatrix](SZGETMatrix.html) |  |
| OFFSET | [Real](Real.html) |  |
| KEEP | [Enum-AcDb3dSolidSlice](Enum-AcDb3dSolidSlice.html) |  |
| --- | --- | --- |
| Returns: | [AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Slice an AcDb3dSolid |

### AcDb3dSolid-SlicesOnCurve

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| CURVE | [AcDbCurve](AcDbCurve.html) |  |
| PITCH | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Make an AcDb3dSolid |

### AcDb3dSolid-SlicesOnVector

| Keys | Types | Help |
| --------- | --------- | --------- |
| BASE | [AcDb3dSolid](AcDb3dSolid.html) |  |
| DIR | [SZGEVector](SZGEVector.html) |  |
| DIST | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDb3dSolid](AcDb3dSolid.html) |
| Help: | Make an AcDb3dSolid |

### AcDb3dSolid-Volume

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [AcDb3dSolid](AcDb3dSolid.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Volume of a Solid |

