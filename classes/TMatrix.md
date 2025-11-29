
# Class:	TMatrix

### Description:

TMatrix Class



### Details:

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [Matrix](Matrix.html) |
| Subclasses: | [TMatrix-Twist](TMatrix-Twist.html) <br> [TMatrix-Mitre](TMatrix-Mitre.html) <br> [TMatrix-Mirror-XY](TMatrix-Mirror-XY.html) <br> [TMatrix-Mirror-X](TMatrix-Mirror-X.html) <br> [TMatrix-Mirror-Y](TMatrix-Mirror-Y.html) <br> [TMatrix-Scale](TMatrix-Scale.html) <br> [TMatrix-Rotation-XAxis](TMatrix-Rotation-XAxis.html) <br> [TMatrix-Rotation-YAxis](TMatrix-Rotation-YAxis.html) <br> [TMatrix-Rotation-ZAxis](TMatrix-Rotation-ZAxis.html) <br> [TMatrix-Translation](TMatrix-Translation.html) <br> [TMatrix-Unit](TMatrix-Unit.html) <br> [TMatrix-Axes](TMatrix-Axes.html) |
| Interfaces: |  |
| Interfaced: | [SZGETMatrix](SZGETMatrix.html), [SZCEPosn](SZCEPosn.html) |
| Abstract?: | No |
| isValue?: | Yes |

### TMatrix-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| X | [Vector](Vector.html) | XAxis Vector |
| Y | [Vector](Vector.html) | YAxis Vector |
| Z | [Vector](Vector.html) | ZAxis Vector |
| POINT | [Point](Point.html) | Origin |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix Creation Routine |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [TMatrix-Origin](#TMatrix-Origin) <br> [TMatrix-Product](#TMatrix-Product) <br> [TMatrix-Relative](#TMatrix-Relative) <br> [TMatrix-Translate](#TMatrix-Translate) <br> [TMatrix-Transpose](#TMatrix-Transpose) <br> [TMatrix-TransposeLT](#TMatrix-TransposeLT) <br> [TMatrix-VectorProduct](#TMatrix-VectorProduct) <br> [TMatrix-XAxis](#TMatrix-XAxis) <br> [TMatrix-YAxis](#TMatrix-YAxis) <br> [TMatrix-ZAxis](#TMatrix-ZAxis) |
| Super: | [Matrix-Determinant](Matrix.html) <br> [Matrix-Orthogonal?](Matrix.html) <br> [List-Make](List.html) <br> [List-Length](List.html) <br> [List->Alist](List.html) <br> [List-IndexSubst](List.html) <br> [List-EndCons](List.html) <br> [List-Addto](List.html) <br> [List-AddtoEnd](List.html) <br> [List-MovetoEnd](List.html) <br> [List-SubLength](List.html) <br> [List-Index](List.html) <br> [List-ItemFill](List.html) <br> [List-IndexFill](List.html) <br> [List-Nth](List.html) <br> [List-Replace](List.html) <br> [List-RemoveItemsAtIndex](List.html) <br> [List-InsertItemsAtIndex](List.html) <br> [List-ItemsAtStart](List.html) <br> [List-ItemsAtEnd](List.html) <br> [List-RemoveLast](List.html) <br> [List-RemoveAtEnd](List.html) <br> [List-RemoveAtStart](List.html) <br> [List-RemoveItem](List.html) <br> [List-RemoveItems](List.html) <br> [List-RemoveNils](List.html) <br> [List-Filter](List.html) <br> [List->Set](List.html) <br> [List-Flatten](List.html) <br> [List-isSubTree?](List.html) <br> [List-Randomise](List.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### TMatrix-Origin

| Keys | Types | Help |
| --------- | --------- | --------- |
| TM | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [Point](Point.html) |
| Help: | Origin of TMatrix |

### TMatrix-Product

| Keys | Types | Help |
| --------- | --------- | --------- |
| M1 | [TMatrix](TMatrix.html) |  |
| M2 | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix Product |

### TMatrix-Relative

| Keys | Types | Help |
| --------- | --------- | --------- |
| P | [TMatrix](TMatrix.html) |  |
| C | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix Relative |

### TMatrix-Translate

| Keys | Types | Help |
| --------- | --------- | --------- |
| M | [TMatrix](TMatrix.html) |  |
| V | [Vector](Vector.html) |  |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TMatrix Translate |

### TMatrix-Transpose

| Keys | Types | Help |
| --------- | --------- | --------- |
| M | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | Transpose of TMatrix |

### TMatrix-TransposeLT

| Keys | Types | Help |
| --------- | --------- | --------- |
| M | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [TMatrix](TMatrix.html) |
| Help: | TransposeLT of TMatrix |

### TMatrix-VectorProduct

| Keys | Types | Help |
| --------- | --------- | --------- |
| M | [TMatrix](TMatrix.html) |  |
| POINT | [Vector](Vector.html) |  |
| DSP | [Logical](Logical.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | TMatrix VectorProduct |

### TMatrix-XAxis

| Keys | Types | Help |
| --------- | --------- | --------- |
| TM | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | XAxis of TMatrix |

### TMatrix-YAxis

| Keys | Types | Help |
| --------- | --------- | --------- |
| TM | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | YAxis of TMatrix |

### TMatrix-ZAxis

| Keys | Types | Help |
| --------- | --------- | --------- |
| TM | [TMatrix](TMatrix.html) |  |
| --- | --- | --- |
| Returns: | [Vector](Vector.html) |
| Help: | ZAxis of TMatrix |

