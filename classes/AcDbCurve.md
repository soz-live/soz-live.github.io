
# Class:	AcDbCurve

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [AcDbEntity](AcDbEntity.html) |
| Subclasses: | [AcDbArc](AcDbArc.html) <br> [AcDb3dPolyline](AcDb3dPolyline.html) <br> [AcDbLine](AcDbLine.html) <br> [AcDbSpline](AcDbSpline.html) <br> [AcDbEllipse](AcDbEllipse.html) <br> [AcDbCircle](AcDbCircle.html) <br> [AcDbPolyline](AcDbPolyline.html) <br> [AcDb2dPolyline](AcDb2dPolyline.html) <br> [AcDbCurve-PlanarClosed](AcDbCurve-PlanarClosed.html) |
| Interfaces: |  |
| Interfaced: |  |
| Abstract?: | Yes |
| isValue?: | No |
| Help: | Base abstract DWG Curve Class |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDbCurve-ClosestPointTo](#AcDbCurve-ClosestPointTo) <br> [AcDbCurve-ClosestPointToProjection](#AcDbCurve-ClosestPointToProjection) <br> [AcDbCurve-EndPoint](#AcDbCurve-EndPoint) <br> [AcDbCurve-EndPoints](#AcDbCurve-EndPoints) <br> [AcDbCurve-Length](#AcDbCurve-Length) <br> [AcDbCurve-MidPoint](#AcDbCurve-MidPoint) <br> [AcDbCurve-NormalVector](#AcDbCurve-NormalVector) <br> [AcDbCurve-PointAtDist](#AcDbCurve-PointAtDist) <br> [AcDbCurve-PointDistFromEnd](#AcDbCurve-PointDistFromEnd) <br> [AcDbCurve-PointDistFromStart](#AcDbCurve-PointDistFromStart) <br> [AcDbCurve-Segments](#AcDbCurve-Segments) <br> [AcDbCurve-StartPoint](#AcDbCurve-StartPoint) <br> [AcDbCurve-TMatrix](#AcDbCurve-TMatrix) <br> [AcDbCurve-TMatrixAtDist](#AcDbCurve-TMatrixAtDist) <br> [AcDbCurve-TMatrixAtPoint](#AcDbCurve-TMatrixAtPoint) <br> [AcDbCurve-TangentVector](#AcDbCurve-TangentVector) <br> [AcDbCurve-isClosed?](#AcDbCurve-isClosed?) <br> [AcDbCurve-isPlanar?](#AcDbCurve-isPlanar?) |
| Super: | [AcDbEntity-Copy](AcDbEntity.html) <br> [AcDbEntity-Move](AcDbEntity.html) <br> [AcDbEntity-Transformby](AcDbEntity.html) <br> [AcDbEntity-IntersectWith](AcDbEntity.html) <br> [AcDbEntity-Layer](AcDbEntity.html) <br> [AcDbEntity-SZCOColor](AcDbEntity.html) <br> [AcDbEntity-Highlight](AcDbEntity.html) <br> [AcDbEntity-SetVisibility](AcDbEntity.html) <br> [AcDbEntity-Space](AcDbEntity.html) <br> [AcDbEntity-InternalCopy](AcDbEntity.html) <br> [AcDbEntity-ExternalCopy](AcDbEntity.html) <br> [AcDbEntity-SetVisual](AcDbEntity.html) <br> [AcDbEntity-Visual](AcDbEntity.html) <br> [AcDbEntity-User_PickList](AcDbEntity.html) <br> [AcDbEntity-User_Pick](AcDbEntity.html) <br> [AcDbEntity-User_PickModel](AcDbEntity.html) <br> [AcDbEntity-User_PickNode](AcDbEntity.html) <br> [AcDbEntity-User_PickSet](AcDbEntity.html) <br> [SZOBObject-AddMetaData](SZOBObject.html) <br> [SZOBObject->SZIX](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDbCurve-ClosestPointTo

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| POINT | [SZGEPoint](SZGEPoint.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | ClosestPointTo of a Curve |

### AcDbCurve-ClosestPointToProjection

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| POINT | [SZGEPoint](SZGEPoint.html) |
| VECTOR | [SZGEVector](SZGEVector.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | ClosestPointtoProjection of a Curve |

### AcDbCurve-EndPoint

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | End Point of a Curve |

### AcDbCurve-EndPoints

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Points](Points.html) |
| Help: | End Points of a Curve |

### AcDbCurve-Length

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Real](Real.html) |
| Help: | Length of a Curve |

### AcDbCurve-MidPoint

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Mid Point of a Curve |

### AcDbCurve-NormalVector

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| POINT | [SZGEPoint](SZGEPoint.html) |
| **---** | **---** |
| Returns: | [Vector](Vector.html) |
| Help: | NormalVector of a Curve |

### AcDbCurve-PointAtDist

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| DIST | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Point At Dist of a Curve |

### AcDbCurve-PointDistFromEnd

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| DIST | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | PointDistFromEnd of a Curve |

### AcDbCurve-PointDistFromStart

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| DIST | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | PointDistFromStart of a Curve |

### AcDbCurve-Segments

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| SEGS | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Points](Points.html) |
| Help: | Segments of a Curve |

### AcDbCurve-StartPoint

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Start Point of a Curve |

### AcDbCurve-TMatrix

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix of a Curve |

### AcDbCurve-TMatrixAtDist

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| DIST | [Real](Real.html) |
| **---** | **---** |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrixAtDist of a Curve |

### AcDbCurve-TMatrixAtPoint

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| POINT | [SZGEPoint](SZGEPoint.html) |
| **---** | **---** |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrixAtPoint of a Curve |

### AcDbCurve-TangentVector

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| POINT | [SZGEPoint](SZGEPoint.html) |
| **---** | **---** |
| Returns: | [Vector](Vector.html) |
| Help: | TangentVector of a Curve |

### AcDbCurve-isClosed?

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Logical](Logical.html) |
| Help: | Closed Predicate |

### AcDbCurve-isPlanar?

| Keys | Types |
| --------- | --------- |
| CURVE | [AcDbCurve](AcDbCurve.html) |
| **---** | **---** |
| Returns: | [Logical](Logical.html) |
| Help: | Planar Predicate |

