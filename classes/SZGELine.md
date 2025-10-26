
# Class:	SZGELine

## Description:

Line CLass


| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [SZGE3dCurve](SZGE3dCurve.html) |
| Subclasses: | [SZGELine-Brace](SZGELine-Brace.html) <br> [SZGELine-MidPoint-Vector-Dist](SZGELine-MidPoint-Vector-Dist.html) <br> [SZGELine-GridLine](SZGELine-GridLine.html) <br> [SZGELine-XLine-2xPlaneIntersect](SZGELine-XLine-2xPlaneIntersect.html) <br> [SZGELine-2xLines-PlaneIntersect](SZGELine-2xLines-PlaneIntersect.html) <br> [SZGELine-LineToPlane-Vertical](SZGELine-LineToPlane-Vertical.html) <br> [SZGELine-PlaneToPlane](SZGELine-PlaneToPlane.html) <br> [SZGELine-PlaneToPlane-Vertical](SZGELine-PlaneToPlane-Vertical.html) <br> [SZGELine-PointToPlane-Vertical](SZGELine-PointToPlane-Vertical.html) <br> [SZGELine-AcDbCircle-Axis](SZGELine-AcDbCircle-Axis.html) <br> [SZGELine-AcDb3dPolyline-Segment](SZGELine-AcDb3dPolyline-Segment.html) <br> [SZGELine-PlaneDistAng](SZGELine-PlaneDistAng.html) <br> [SZGELine-Planes-Intersect](SZGELine-Planes-Intersect.html) <br> [SZGELine-Points-Offsets](SZGELine-Points-Offsets.html) <br> [SZGELine-PointVector-PlaneToPlane](SZGELine-PointVector-PlaneToPlane.html) <br> [SZGELine-PointVector-Plane](SZGELine-PointVector-Plane.html) <br> [SZGELine-PointVector-Dist](SZGELine-PointVector-Dist.html) <br> [SZGELine-PointVector](SZGELine-PointVector.html) |
| Interfaces: | [Line](Line.html) |
| Interfaced: | [AcDbXline](AcDbXline.html), [AcDbRay](AcDbRay.html), [AcDbLine](AcDbLine.html) |
| Abstract?: | No |
| isValue?: | Yes |

### SZGELine-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| POINT0 | [SZGEPoint](SZGEPoint.html) |  |
| POINT1 | [SZGEPoint](SZGEPoint.html) |  |
| --- | --- | --- |
| Returns: | [SZGELine](SZGELine.html) |
| Help: | Makes a Line |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [SZGELine-BaryComb](#SZGELine-BaryComb) <br> [SZGELine-EndPoint](#SZGELine-EndPoint) <br> [SZGELine-Length](#SZGELine-Length) <br> [SZGELine-MidPoint](#SZGELine-MidPoint) <br> [SZGELine-StartPoint](#SZGELine-StartPoint) <br> [SZGELine-TMatrix](#SZGELine-TMatrix) <br> [SZGELine-User_Pick](#SZGELine-User_Pick) <br> [SZGELine-Value](#SZGELine-Value) <br> [SZGELine-Vector](#SZGELine-Vector) |
| Super: | [SZGE3dCurve-Make](SZGE3dCurve.html) <br> [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### SZGELine-BaryComb

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| BC | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [Point](Point.html) |
| Help: | BaryComb of a SZGELine |

### SZGELine-EndPoint

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [Point](Point.html) |
| Help: | EndPoint of a SZGELine |

### SZGELine-Length

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Length of a SZGELine |

### SZGELine-MidPoint

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [Point](Point.html) |
| Help: | MidPoint of a SZGELine |

### SZGELine-StartPoint

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [Point](Point.html) |
| Help: | StartPoint of a SZGELine |

### SZGELine-TMatrix

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix of a SZGELine |

### SZGELine-User_Pick

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [SZGELine](SZGELine.html) |
| Help: | User_Pick |

### SZGELine-Value

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [Line](Line.html) |
| Help: | Value of a SZGELine |

### SZGELine-Vector

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [SZGELine](SZGELine.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector of a SZGELine |

