---------

# Class:	AcDbLine

| Fields | Values |
| --------- | --------- |
| Superclass: | [AcDbCurve](AcDbCurve.html) |
| Subclasses: | [SZCELine](SZCELine.html) |
| Interfaces: | [Line](Line.html), [SZGELine](SZGELine.html) |
| Interfaced: | [SZCELinear](SZCELinear.html) |
| Abstract?: | No |
| isValue?: | No |
| Help: | AcDbLine Class |

### AcDbLine-Make

| Keys | Types |
| --------- | --------- |
| SPACE | [AcDbBlock](AcDbBlock.html) |
| LINE | [SZGELine](SZGELine.html) |
| **---** | **---** |
| Returns: | [AcDbLine](AcDbLine.html) |
| Help: | Make a AcDbLine |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDbLine-EndPoint](#AcDbLine-EndPoint) <br> [AcDbLine-Length](#AcDbLine-Length) <br> [AcDbLine-Line](#AcDbLine-Line) <br> [AcDbLine-Points](#AcDbLine-Points) <br> [AcDbLine-StartPoint](#AcDbLine-StartPoint) <br> [AcDbLine-TMatrix](#AcDbLine-TMatrix) <br> [AcDbLine-User_PickMember](#AcDbLine-User_PickMember) <br> [AcDbLine-Vector](#AcDbLine-Vector) |
| Super: | [AcDbCurve-isClosed?](AcDbCurve.html) <br> [AcDbCurve-isPlanar?](AcDbCurve.html) <br> [AcDbCurve-EndPoints](AcDbCurve.html) <br> [AcDbCurve-Length](AcDbCurve.html) <br> [AcDbCurve-PointAtDist](AcDbCurve.html) <br> [AcDbCurve-StartPoint](AcDbCurve.html) <br> [AcDbCurve-EndPoint](AcDbCurve.html) <br> [AcDbCurve-MidPoint](AcDbCurve.html) <br> [AcDbCurve-PointDistFromStart](AcDbCurve.html) <br> [AcDbCurve-PointDistFromEnd](AcDbCurve.html) <br> [AcDbCurve-ClosestPointTo](AcDbCurve.html) <br> [AcDbCurve-ClosestPointToProjection](AcDbCurve.html) <br> [AcDbCurve-TangentVector](AcDbCurve.html) <br> [AcDbCurve-NormalVector](AcDbCurve.html) <br> [AcDbCurve-TMatrixAtPoint](AcDbCurve.html) <br> [AcDbCurve-TMatrixAtDist](AcDbCurve.html) <br> [AcDbCurve-Segments](AcDbCurve.html) <br> [AcDbCurve-TMatrix](AcDbCurve.html) <br> [AcDbEntity-Copy](AcDbEntity.html) <br> [AcDbEntity-Move](AcDbEntity.html) <br> [AcDbEntity-Transformby](AcDbEntity.html) <br> [AcDbEntity-IntersectWith](AcDbEntity.html) <br> [AcDbEntity-Layer](AcDbEntity.html) <br> [AcDbEntity-SetVisibility](AcDbEntity.html) <br> [AcDbEntity-Space](AcDbEntity.html) <br> [AcDbEntity-InternalCopy](AcDbEntity.html) <br> [AcDbEntity-ExternalCopy](AcDbEntity.html) <br> [AcDbEntity-SetVisual](AcDbEntity.html) <br> [AcDbEntity-Visual](AcDbEntity.html) <br> [AcDbEntity-User_PickList](AcDbEntity.html) <br> [AcDbEntity-User_Pick](AcDbEntity.html) <br> [AcDbEntity-User_PickModel](AcDbEntity.html) <br> [AcDbEntity-User_PickNode](AcDbEntity.html) <br> [AcDbEntity-User_PickSet](AcDbEntity.html) <br> [SZOBObject-AddMetaData](SZOBObject.html) <br> [SZOBObject->SZIX](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDbLine-EndPoint

| Keys | Types |
| --------- | --------- |
| E | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | EndPoint of a AcDbLine |

### AcDbLine-Length

| Keys | Types |
| --------- | --------- |
| E | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [Real](Real.html) |
| Help: | Length of a AcDbLine |

### AcDbLine-Line

| Keys | Types |
| --------- | --------- |
| O | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [Line](Line.html) |
| Help: | Line of a AcDbLine |

### AcDbLine-Points

| Keys | Types |
| --------- | --------- |
| O | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [List:Point](Point.html) |
| Help: | Line of a AcDbLine |

### AcDbLine-StartPoint

| Keys | Types |
| --------- | --------- |
| E | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | StartPoint of a AcDbLine |

### AcDbLine-TMatrix

| Keys | Types |
| --------- | --------- |
| E | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix of a AcDbLine |

### AcDbLine-User_PickMember

| Keys | Types |
| --------- | --------- |
| USER | [User](User.html) |
| **---** | **---** |
| Returns: | [AcDbLine](AcDbLine.html) |
| Help: | User_PickMember |

### AcDbLine-Vector

| Keys | Types |
| --------- | --------- |
| O | [AcDbLine](AcDbLine.html) |
| **---** | **---** |
| Returns: | [Vector](Vector.html) |
| Help: | Vector of a AcDbLine |
