
# Class:	Line

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [3dCurve](3dCurve.html) |
| Subclasses: | [Line-Segment](Line-Segment.html) |
| Interfaces: |  |
| Interfaced: | [SZGELine](SZGELine.html), [AcDbXline](AcDbXline.html), [AcDbRay](AcDbRay.html), [AcDbLine](AcDbLine.html) |
| Abstract?: | No |
| isValue?: | Yes |
| Help: | Line Class |

### Line-Make

| Keys | Types |
| --------- | --------- |
| POINT0 | [Point](Point.html) |
| POINT1 | [Point](Point.html) |
| **---** | **---** |
| Returns: | [Line](Line.html) |
| Help: | Make a Line |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [Line-Axes](#Line-Axes) <br> [Line-BaryComb](#Line-BaryComb) <br> [Line-EndPoint](#Line-EndPoint) <br> [Line-FaceIntersect](#Line-FaceIntersect) <br> [Line-Flatten](#Line-Flatten) <br> [Line-Length](#Line-Length) <br> [Line-MidPoint](#Line-MidPoint) <br> [Line-PlaneIntersect](#Line-PlaneIntersect) <br> [Line-PointAtDistance](#Line-PointAtDistance) <br> [Line-StartPoint](#Line-StartPoint) <br> [Line-TMatrix](#Line-TMatrix) <br> [Line-Value](#Line-Value) <br> [Line-Vector](#Line-Vector) |
| Super: | [List-Make](List.html) <br> [List-Length](List.html) <br> [List->Alist](List.html) <br> [List-IndexSubst](List.html) <br> [List-EndCons](List.html) <br> [List-Addto](List.html) <br> [List-AddtoEnd](List.html) <br> [List-SubLength](List.html) <br> [List-Index](List.html) <br> [List-ItemFill](List.html) <br> [List-IndexFill](List.html) <br> [List-Nth](List.html) <br> [List-Replace](List.html) <br> [List-RemoveItemsAtIndex](List.html) <br> [List-InsertItemsAtIndex](List.html) <br> [List-ItemsAtStart](List.html) <br> [List-ItemsAtEnd](List.html) <br> [List-RemoveLast](List.html) <br> [List-RemoveAtEnd](List.html) <br> [List-RemoveAtStart](List.html) <br> [List-RemoveItem](List.html) <br> [List-RemoveItems](List.html) <br> [List-RemoveNils](List.html) <br> [List-Filter](List.html) <br> [List->Set](List.html) <br> [List-Flatten](List.html) <br> [List-isSubTree?](List.html) <br> [List-Randomise](List.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### Line-Axes

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Axes](Axes.html) |
| Help: | Line Axes |

### Line-BaryComb

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| COEFF | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line BaryComb |

### Line-EndPoint

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line EndPoint |

### Line-FaceIntersect

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| FACE | [Face](Face.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line FaceIntersect |

### Line-Flatten

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Line](Line.html) |
| Help: | Line Flattened |

### Line-Length

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Real](Real.html) |
| Help: | Line Length |

### Line-MidPoint

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line MidPoint |

### Line-PlaneIntersect

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| PLANE | [Plane](Plane.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line PlaneIntersect |

### Line-PointAtDistance

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| D | [Real](Real.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line PointAtDistance |

### Line-StartPoint

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Point](Point.html) |
| Help: | Line StartPoint |

### Line-TMatrix

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | Line TMatrix |

### Line-Value

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Line](Line.html) |
| Help: | Line Value |

### Line-Vector

| Keys | Types |
| --------- | --------- |
| L | [Line](Line.html) |
| **---** | **---** |
| Returns: | [Vector](Vector.html) |
| Help: | Line Vector |

