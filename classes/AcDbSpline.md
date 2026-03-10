
# Class:	AcDbSpline

### Description:

AcDbSpline Class



### Details:

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [AcDbCurve](AcDbCurve.html) |
| Subclasses: | [AcDbHelix](AcDbHelix.html) |
| Interfaces: |  |
| Interfaced: | [AcDbCurve-PlanarClosed](AcDbCurve-PlanarClosed.html) |
| Abstract?: | No |
| isValue?: | No |

### AcDbSpline-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| SPACE | [AcDbBlock](AcDbBlock.html) | Make within Block |
| FITPTS | [SZGEPoints](SZGEPoints.html) |  |
| STARTTAN | [SZGEVector](SZGEVector.html) |  |
| ENDTAN | [SZGEVector](SZGEVector.html) |  |
| FITTOL | [Number](Number.html) |  |
| CLOSED | [Boolean](Boolean.html) |  |
| | | |
| Returns: | [AcDbSpline](AcDbSpline.html) | |
| Help: | | Make an AcDbSpline |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDbSpline-Closed](#AcDbSpline-Closed) <br> [AcDbSpline-EndTangent](#AcDbSpline-EndTangent) <br> [AcDbSpline-FitPoints](#AcDbSpline-FitPoints) <br> [AcDbSpline-FitTolerance](#AcDbSpline-FitTolerance) <br> [AcDbSpline-StartTangent](#AcDbSpline-StartTangent) |
| Super: | [AcDbCurve-isClosed?](AcDbCurve.html) <br> [AcDbCurve-isPlanar?](AcDbCurve.html) <br> [AcDbCurve-EndPoints](AcDbCurve.html) <br> [AcDbCurve-Length](AcDbCurve.html) <br> [AcDbCurve-PointAtDist](AcDbCurve.html) <br> [AcDbCurve-PointAtRatio](AcDbCurve.html) <br> [AcDbCurve-StartPoint](AcDbCurve.html) <br> [AcDbCurve-EndPoint](AcDbCurve.html) <br> [AcDbCurve-MidPoint](AcDbCurve.html) <br> [AcDbCurve-PointDistFromStart](AcDbCurve.html) <br> [AcDbCurve-PointDistFromEnd](AcDbCurve.html) <br> [AcDbCurve-ClosestPointTo](AcDbCurve.html) <br> [AcDbCurve-ClosestPointToProjection](AcDbCurve.html) <br> [AcDbCurve-TangentVector](AcDbCurve.html) <br> [AcDbCurve-NormalVector](AcDbCurve.html) <br> [AcDbCurve-TMatrixAtPoint](AcDbCurve.html) <br> [AcDbCurve-TMatrixAtDist](AcDbCurve.html) <br> [AcDbCurve-Segments](AcDbCurve.html) <br> [AcDbCurve-Points](AcDbCurve.html) <br> [AcDbCurve-TMatrix](AcDbCurve.html) <br> [AcDbEntity-Copy](AcDbEntity.html) <br> [AcDbEntity-Move](AcDbEntity.html) <br> [AcDbEntity-Transformby](AcDbEntity.html) <br> [AcDbEntity-IntersectWith](AcDbEntity.html) <br> [AcDbEntity-Layer](AcDbEntity.html) <br> [AcDbEntity-SetLayer](AcDbEntity.html) <br> [AcDbEntity-SZCOColor](AcDbEntity.html) <br> [AcDbEntity-Highlight](AcDbEntity.html) <br> [AcDbEntity-SetVisibility](AcDbEntity.html) <br> [AcDbEntity-Space](AcDbEntity.html) <br> [AcDbEntity-InternalCopy](AcDbEntity.html) <br> [AcDbEntity-ExternalCopy](AcDbEntity.html) <br> [AcDbEntity-SetVisual](AcDbEntity.html) <br> [AcDbEntity-Visual](AcDbEntity.html) <br> [AcDbEntity-User_PickList](AcDbEntity.html) <br> [AcDbEntity-User_Pick](AcDbEntity.html) <br> [AcDbEntity-User_PickModel](AcDbEntity.html) <br> [AcDbEntity-User_PickNode](AcDbEntity.html) <br> [AcDbEntity-User_PickSet](AcDbEntity.html) <br> [SZOBObject-IndexOfXOBJS](SZOBObject.html) <br> [SZOBObject-AddIOBJ](SZOBObject.html) <br> [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDbSpline-Closed

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDbSpline](AcDbSpline.html) |  |
| | | |
| Returns: | [Boolean](Boolean.html) | |
| Help: | | Closed of an AcDbSpline |

### AcDbSpline-EndTangent

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDbSpline](AcDbSpline.html) |  |
| | | |
| Returns: | [Vector](Vector.html) | |
| Help: | | EndTangent of an AcDbSpline |

### AcDbSpline-FitPoints

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDbSpline](AcDbSpline.html) |  |
| | | |
| Returns: | [Points](Points.html) | |
| Help: | | FitPoints of an AcDbSpline |

### AcDbSpline-FitTolerance

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDbSpline](AcDbSpline.html) |  |
| | | |
| Returns: | [Number](Number.html) | |
| Help: | | FitTolerance of an AcDbSpline |

### AcDbSpline-StartTangent

| Keys | Types | Help |
| --------- | --------- | --------- |
| E | [AcDbSpline](AcDbSpline.html) |  |
| | | |
| Returns: | [Vector](Vector.html) | |
| Help: | | StartTangent of an AcDbSpline |

