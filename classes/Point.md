
# Class:	Point

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [Vector](Vector.html) |
| Subclasses: | [Point2D](Point2D.html) <br> [Point-Spherical](Point-Spherical.html) |
| Interfaces: |  |
| Interfaced: | [SZGEPoint](SZGEPoint.html), [AcDbPoint](AcDbPoint.html) |
| Abstract?: | No |
| isValue?: | Yes |
| Help: | Point Class |

### Point-Make

| Keys | Types |
| --------- | --------- |
| X | [Real](Real.html) |
| Y | [Real](Real.html) |
| Z | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Make a Point |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [Point->Points](#Point->Points) <br> [Point-Flatten](#Point-Flatten) <br> [Point-LinePerpPosn](#Point-LinePerpPosn) <br> [Point-OnLine?](#Point-OnLine?) <br> [Point-OnPlane](#Point-OnPlane) <br> [Point-Origin](#Point-Origin) <br> [Point-Reset](#Point-Reset) <br> [Point-TransformBy](#Point-TransformBy) <br> [Point-WithinRectangle?](#Point-WithinRectangle?) <br> [Point-WithinTriangle?](#Point-WithinTriangle?) <br> [Point-onFace?](#Point-onFace?) |
| Super: | [Vector-Make](Vector.html) <br> [Vector-X](Vector.html) <br> [Vector-Y](Vector.html) <br> [Vector-Z](Vector.html) <br> [Vector->Vector2D](Vector.html) <br> [Vector->Vector3D](Vector.html) <br> [Vector-CrossProduct](Vector.html) <br> [Vector-DotProduct](Vector.html) <br> [Vector-Normal](Vector.html) <br> [Vector-Sum](Vector.html) <br> [Vector-Product](Vector.html) <br> [Vector-Subtract](Vector.html) <br> [Vector-Negate](Vector.html) <br> [Vector-Scalar](Vector.html) <br> [Vector-Length](Vector.html) <br> [Vector-Angle](Vector.html) <br> [Vector-Equal?](Vector.html) <br> [Vector-Zero](Vector.html) <br> [Vector-XAxis](Vector.html) <br> [Vector-YAxis](Vector.html) <br> [Vector-ZAxis](Vector.html) <br> [Vector-OrthoVector](Vector.html) <br> [Vector-TransformBy](Vector.html) <br> [Vector->Axes](Vector.html) <br> [Vector-User_Edit](Vector.html) <br> [List-Make](List.html) <br> [List-Length](List.html) <br> [List->Alist](List.html) <br> [List-IndexSubst](List.html) <br> [List-EndCons](List.html) <br> [List-Addto](List.html) <br> [List-AddtoEnd](List.html) <br> [List-SubLength](List.html) <br> [List-Index](List.html) <br> [List-ItemFill](List.html) <br> [List-IndexFill](List.html) <br> [List-Nth](List.html) <br> [List-Replace](List.html) <br> [List-RemoveItemsAtIndex](List.html) <br> [List-InsertItemsAtIndex](List.html) <br> [List-ItemsAtStart](List.html) <br> [List-ItemsAtEnd](List.html) <br> [List-RemoveLast](List.html) <br> [List-RemoveAtEnd](List.html) <br> [List-RemoveAtStart](List.html) <br> [List-RemoveItem](List.html) <br> [List-RemoveItems](List.html) <br> [List-RemoveNils](List.html) <br> [List-Filter](List.html) <br> [List->Set](List.html) <br> [List-Flatten](List.html) <br> [List-isSubTree?](List.html) <br> [List-Randomise](List.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### Point->Points

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Points](Points.html) |
| Help: | Convert to Points |

### Point-Flatten

| Keys | Types |
| --------- | --------- |
| V | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Flatten Point |

### Point-LinePerpPosn

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| LPT0 | [Point](Point.html) |
| LPT1 | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line Perp Posn |

### Point-OnLine?

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| LINE | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Logical](Logical.html) |
| Help: | Point OnLine? |

### Point-OnPlane

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| PLANE | [Plane](Plane.html) |
| DIR | [Vector](Vector.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Point on a Plane |

### Point-Origin

| Keys | Types |
| --------- | --------- |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Origin Point |

### Point-Reset

| Keys | Types |
| --------- | --------- |
| O | [Point](Point.html) |
| NEW | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Reset a Point |

### Point-TransformBy

| Keys | Types |
| --------- | --------- |
| PT | [Point](Point.html) |
| TM | [TMatrix](TMatrix.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Point TransformBy |

### Point-WithinRectangle?

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| POINT1 | [Point](Point.html) |
| POINT2 | [Point](Point.html) |
| POINT3 | [Point](Point.html) |
| POINT4 | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Logical](Logical.html) |
| Help: | Point WithinRectangle? |

### Point-WithinTriangle?

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| POINT1 | [Point](Point.html) |
| POINT2 | [Point](Point.html) |
| POINT3 | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Logical](Logical.html) |
| Help: | Point WithinTriangle? |

### Point-onFace?

| Keys | Types |
| --------- | --------- |
| POINT | [Point](Point.html) |
| FACE | [Face](Face.html) |
| **---** | **---** |
| Returns: | [Logical](Logical.html) |
| Help: | Point onFace? |

