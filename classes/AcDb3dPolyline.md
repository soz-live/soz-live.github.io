
# Class:	AcDb3dPolyline

### Description:

AcDb3dPolyline Class



### Details:

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [AcDbCurve](AcDbCurve.html) |
| Subclasses: | [SZDOLink](SZDOLink.html) <br> [SZLVLink](SZLVLink.html) <br> [SZCE3dCurve](SZCE3dCurve.html) <br> [AcDb3dPolyline-Flatten](AcDb3dPolyline-Flatten.html) |
| Interfaces: | [SZGEPoints](SZGEPoints.html), [Points](Points.html) |
| Interfaced: | [AcDbCurve-PlanarClosed](AcDbCurve-PlanarClosed.html) |
| Abstract?: | No |
| isValue?: | No |

### AcDb3dPolyline-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| SPACE | [AcDbBlock](AcDbBlock.html) | Make within Block |
| POINTS | [SZGEPoints](SZGEPoints.html) |  |
| CLOSED | [Boolean](Boolean.html) |  |
| POLYTYPE | [Enum-AcDb3dPolylineType](Enum-AcDb3dPolylineType.html) |  |
| --- | --- | --- |
| Returns: | [AcDb3dPolyline](AcDb3dPolyline.html) |
| Help: | Make an AcDb3dPolyline |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDb3dPolyline-Closed](#AcDb3dPolyline-Closed) <br> [AcDb3dPolyline-Fillet](#AcDb3dPolyline-Fillet) <br> [AcDb3dPolyline-Length](#AcDb3dPolyline-Length) <br> [AcDb3dPolyline-LineSegments](#AcDb3dPolyline-LineSegments) <br> [AcDb3dPolyline-Points](#AcDb3dPolyline-Points) <br> [AcDb3dPolyline-PolyType](#AcDb3dPolyline-PolyType) <br> [AcDb3dPolyline-RadiiFillet](#AcDb3dPolyline-RadiiFillet) <br> [AcDb3dPolyline-RadiusFillet](#AcDb3dPolyline-RadiusFillet) |
| Super: | [AcDbCurve-isClosed?](AcDbCurve.html) <br> [AcDbCurve-isPlanar?](AcDbCurve.html) <br> [AcDbCurve-EndPoints](AcDbCurve.html) <br> [AcDbCurve-Length](AcDbCurve.html) <br> [AcDbCurve-PointAtDist](AcDbCurve.html) <br> [AcDbCurve-PointAtRatio](AcDbCurve.html) <br> [AcDbCurve-StartPoint](AcDbCurve.html) <br> [AcDbCurve-EndPoint](AcDbCurve.html) <br> [AcDbCurve-MidPoint](AcDbCurve.html) <br> [AcDbCurve-PointDistFromStart](AcDbCurve.html) <br> [AcDbCurve-PointDistFromEnd](AcDbCurve.html) <br> [AcDbCurve-ClosestPointTo](AcDbCurve.html) <br> [AcDbCurve-ClosestPointToProjection](AcDbCurve.html) <br> [AcDbCurve-TangentVector](AcDbCurve.html) <br> [AcDbCurve-NormalVector](AcDbCurve.html) <br> [AcDbCurve-TMatrixAtPoint](AcDbCurve.html) <br> [AcDbCurve-TMatrixAtDist](AcDbCurve.html) <br> [AcDbCurve-Segments](AcDbCurve.html) <br> [AcDbCurve-TMatrix](AcDbCurve.html) <br> [AcDbEntity-Copy](AcDbEntity.html) <br> [AcDbEntity-Move](AcDbEntity.html) <br> [AcDbEntity-Transformby](AcDbEntity.html) <br> [AcDbEntity-IntersectWith](AcDbEntity.html) <br> [AcDbEntity-Layer](AcDbEntity.html) <br> [AcDbEntity-SetLayer](AcDbEntity.html) <br> [AcDbEntity-SZCOColor](AcDbEntity.html) <br> [AcDbEntity-Highlight](AcDbEntity.html) <br> [AcDbEntity-SetVisibility](AcDbEntity.html) <br> [AcDbEntity-Space](AcDbEntity.html) <br> [AcDbEntity-InternalCopy](AcDbEntity.html) <br> [AcDbEntity-ExternalCopy](AcDbEntity.html) <br> [AcDbEntity-SetVisual](AcDbEntity.html) <br> [AcDbEntity-Visual](AcDbEntity.html) <br> [AcDbEntity-User_PickList](AcDbEntity.html) <br> [AcDbEntity-User_Pick](AcDbEntity.html) <br> [AcDbEntity-User_PickModel](AcDbEntity.html) <br> [AcDbEntity-User_PickNode](AcDbEntity.html) <br> [AcDbEntity-User_PickSet](AcDbEntity.html) <br> [SZOBObject-IndexOfXOBJS](SZOBObject.html) <br> [SZOBObject-AddIOBJ](SZOBObject.html) <br> [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDb3dPolyline-Closed

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| --- | --- | --- |
| Returns: | [Boolean](Boolean.html) |
| Help: | Closed of an AcDb3dPolyline |

### AcDb3dPolyline-Fillet

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| RADII | [List:Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDbCurve](AcDbCurve.html) |
| Help: | Filleted AcDb3dPolyline |

### AcDb3dPolyline-Length

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Length of an AcDb3dPolyline |

### AcDb3dPolyline-LineSegments

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| --- | --- | --- |
| Returns: | [Lines](Lines.html) |
| Help: | Line Segments of an AcDb3dPolyline |

### AcDb3dPolyline-Points

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| --- | --- | --- |
| Returns: | [Points](Points.html) |
| Help: | Points of an AcDb3dPolyline |

### AcDb3dPolyline-PolyType

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| --- | --- | --- |
| Returns: | [Enum-AcDb3dPolylineType](Enum-AcDb3dPolylineType.html) |
| Help: | 3dPolylineTypeEnum of an AcDb3dPolyline |

### AcDb3dPolyline-RadiiFillet

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| RADII | [List:Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDbCurve](AcDbCurve.html) |
| Help: | Filleted AcDb3dPolyline using radii |

### AcDb3dPolyline-RadiusFillet

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDb3dPolyline](AcDb3dPolyline.html) |  |
| RADIUS | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDbCurve](AcDbCurve.html) |
| Help: | Filleted AcDb3dPolyline using radius |

