
# Class:	Vector

### Description:

Vector Class



### Details:

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [Reals](Reals.html) |
| Subclasses: | [Point](Point.html) <br> [Orientation](Orientation.html) <br> [Vector2D](Vector2D.html) |
| Interfaces: |  |
| Interfaced: | [SZGEVector](SZGEVector.html), [SZOBAnimate-Effect-Vector](SZOBAnimate-Effect-Vector.html) |
| Abstract?: | No |
| isValue?: | Yes |

### Vector-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| X | [Real](Real.html) |  |
| Y | [Real](Real.html) |  |
| Z | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Creates a Vector of X Y Z values |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [Vector->Axes](#Vector->Axes) <br> [Vector->Vector2D](#Vector->Vector2D) <br> [Vector->Vector3D](#Vector->Vector3D) <br> [Vector-Angle](#Vector-Angle) <br> [Vector-CrossProduct](#Vector-CrossProduct) <br> [Vector-DotProduct](#Vector-DotProduct) <br> [Vector-Equal?](#Vector-Equal?) <br> [Vector-Length](#Vector-Length) <br> [Vector-Negate](#Vector-Negate) <br> [Vector-Normal](#Vector-Normal) <br> [Vector-OrthoVector](#Vector-OrthoVector) <br> [Vector-Product](#Vector-Product) <br> [Vector-Scalar](#Vector-Scalar) <br> [Vector-Subtract](#Vector-Subtract) <br> [Vector-Sum](#Vector-Sum) <br> [Vector-TransformBy](#Vector-TransformBy) <br> [Vector-User_Edit](#Vector-User_Edit) <br> [Vector-X](#Vector-X) <br> [Vector-XAxis](#Vector-XAxis) <br> [Vector-Y](#Vector-Y) <br> [Vector-YAxis](#Vector-YAxis) <br> [Vector-Z](#Vector-Z) <br> [Vector-ZAxis](#Vector-ZAxis) <br> [Vector-Zero](#Vector-Zero) |
| Super: | [List-Make](List.html) <br> [List-Length](List.html) <br> [List->Alist](List.html) <br> [List-IndexSubst](List.html) <br> [List-EndCons](List.html) <br> [List-Addto](List.html) <br> [List-AddtoEnd](List.html) <br> [List-MovetoEnd](List.html) <br> [List-SubLength](List.html) <br> [List-Index](List.html) <br> [List-ItemFill](List.html) <br> [List-IndexFill](List.html) <br> [List-Nth](List.html) <br> [List-Replace](List.html) <br> [List-RemoveItemsAtIndex](List.html) <br> [List-InsertItemsAtIndex](List.html) <br> [List-ItemsAtStart](List.html) <br> [List-ItemsAtEnd](List.html) <br> [List-RemoveLast](List.html) <br> [List-RemoveAtEnd](List.html) <br> [List-RemoveAtStart](List.html) <br> [List-RemoveItem](List.html) <br> [List-RemoveItems](List.html) <br> [List-RemoveNils](List.html) <br> [List-Filter](List.html) <br> [List->Set](List.html) <br> [List-Flatten](List.html) <br> [List-isSubTree?](List.html) <br> [List-Randomise](List.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### Vector->Axes

| Keys | Types | Help |
| --------- | --------- | --------- |
| ZAXIS | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Axes](Axes.html) |
| Help: | Convert to Axes |

### Vector->Vector2D

| Keys | Types | Help |
| --------- | --------- | --------- |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector2D](Vector2D.html) |
| Help: | Convert Vector to Vector2D |

### Vector->Vector3D

| Keys | Types | Help |
| --------- | --------- | --------- |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Convert Vector to Vector3D |

### Vector-Angle

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Rad](Rad.html) |
| Help: | Vector Angle |

### Vector-CrossProduct

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector CrossProduct |

### Vector-DotProduct

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Vector DotProduct |

### Vector-Equal?

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Logical](Logical.html) |
| Help: | Vector Equal? |

### Vector-Length

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Vector Length |

### Vector-Negate

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector Negate |

### Vector-Normal

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector Normal |

### Vector-OrthoVector

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | OrthoVector |

### Vector-Product

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector Product |

### Vector-Scalar

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Real](Real.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector Scalar |

### Vector-Subtract

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector Subtract |

### Vector-Sum

| Keys | Types | Help |
| --------- | --------- | --------- |
| U | [Vector](Vector.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector Sum |

### Vector-TransformBy

| Keys | Types | Help |
| --------- | --------- | --------- |
| V | [Vector](Vector.html) |  |
| TM | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Vector TransformBy |

### Vector-User_Edit

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Edit a Vector |

### Vector-X

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | X Coord of Vector |

### Vector-XAxis

| Keys | Types | Help |
| --------- | --------- | --------- |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | XAxis Vector |

### Vector-Y

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Y Coord of Vector |

### Vector-YAxis

| Keys | Types | Help |
| --------- | --------- | --------- |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | YAxis Vector |

### Vector-Z

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [Real](Real.html) |
| Help: | Z Coord of Vector |

### Vector-ZAxis

| Keys | Types | Help |
| --------- | --------- | --------- |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | ZAxis Vector |

### Vector-Zero

| Keys | Types | Help |
| --------- | --------- | --------- |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | Zero Vector |

