
# Class:	List

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [T](T.html) |
| Subclasses: | [Set](Set.html) <br> [Array](Array.html) <br> [Pair](Pair.html) <br> [Cons](Cons.html) <br> [Tree](Tree.html) |
| Interfaces: |  |
| Interfaced: | [NIL](NIL.html), [SZLPList](SZLPList.html), [SZGEObjects](SZGEObjects.html), [SZCOObjects](SZCOObjects.html) |
| Abstract?: | Yes |
| isValue?: | Yes |
| Help: | List Class |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [List->Set](#List->Set) <br> [List-Addto](#List-Addto) <br> [List-AddtoEnd](#List-AddtoEnd) <br> [List-EndCons](#List-EndCons) <br> [List-Filter](#List-Filter) <br> [List-Flatten](#List-Flatten) <br> [List-Index](#List-Index) <br> [List-IndexFill](#List-IndexFill) <br> [List-IndexSubst](#List-IndexSubst) <br> [List-InsertItemsAtIndex](#List-InsertItemsAtIndex) <br> [List-ItemFill](#List-ItemFill) <br> [List-ItemsAtEnd](#List-ItemsAtEnd) <br> [List-ItemsAtStart](#List-ItemsAtStart) <br> [List-Length](#List-Length) <br> [List-MovetoEnd](#List-MovetoEnd) <br> [List-Nth](#List-Nth) <br> [List-Randomise](#List-Randomise) <br> [List-RemoveAtEnd](#List-RemoveAtEnd) <br> [List-RemoveAtStart](#List-RemoveAtStart) <br> [List-RemoveItem](#List-RemoveItem) <br> [List-RemoveItems](#List-RemoveItems) <br> [List-RemoveItemsAtIndex](#List-RemoveItemsAtIndex) <br> [List-RemoveLast](#List-RemoveLast) <br> [List-RemoveNils](#List-RemoveNils) <br> [List-Replace](#List-Replace) <br> [List-SubLength](#List-SubLength) |
| Super: | [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### List->Set

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| --- | --- | --- |
| Returns: | [Set](Set.html) |
| Help: | Removes Duplicates from a List (Makes a Set) |

### List-Addto

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| V | [Atom](Atom.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Adds element to a list if not in there already |

### List-AddtoEnd

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| V | [Atom](Atom.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Adds element to End of a list if not in there already |

### List-EndCons

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| V | [Atom](Atom.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Adds element to the end of a List |

### List-Filter

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| FILTER | [Predicate](Predicate.html) |  |
| PARAM | [List](List.html) |  |
| INVERT | [Logical](Logical.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Filters elements of a List |

### List-Flatten

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Returns a flattened List (no sub-lists) |

### List-Index

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| ITEM | [SZOBObject](SZOBObject.html) |  |
| --- | --- | --- |
| Returns: | [Integer](Integer.html) |
| Help: | Item's Index in a List |

### List-IndexFill

| Keys | Types | Help |
| --------- | --------- | --------- |
| NO | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Makes a list of Indices, NO long |

### List-IndexSubst

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| INDEX | [Integer](Integer.html) |  |
| VALUE | [T](T.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Substitutes a value at a given index in a List |

### List-InsertItemsAtIndex

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| IND | [Integer](Integer.html) |  |
| VALUES | [List:SZOBObject](SZOBObject.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Insert Items At Index in a List |

### List-ItemFill

| Keys | Types | Help |
| --------- | --------- | --------- |
| NO | [Integer](Integer.html) |  |
| ITEM | [T](T.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Makes a list of Items, NO long |

### List-ItemsAtEnd

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| NO | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Gets last no items of a List |

### List-ItemsAtStart

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| NO | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Gets first no items of a List |

### List-Length

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [List](List.html) |  |
| --- | --- | --- |
| Returns: | [Integer](Integer.html) |
| Help: | Length of a List |

### List-MovetoEnd

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| V | [Atom](Atom.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Moves element to End of a list if not in there already |

### List-Nth

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| INDEX | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [SZOBObject](SZOBObject.html) |
| Help: | Item of a List |

### List-Randomise

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Randomise a List |

### List-RemoveAtEnd

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| NO | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes last elements of a List |

### List-RemoveAtStart

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| NO | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes start elements of a List |

### List-RemoveItem

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| ITEM | [T](T.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes elements of a List |

### List-RemoveItems

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| ITEMS | [List:T](T.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes elements of a List |

### List-RemoveItemsAtIndex

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| IND | [Integer](Integer.html) |  |
| NO | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes Items At an Index in a List |

### List-RemoveLast

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes last element of a List |

### List-RemoveNils

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Removes NIL elements of a List |

### List-Replace

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| OLD | [SZOBObject](SZOBObject.html) |  |
| NEW | [SZOBObject](SZOBObject.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Substitutes a value at a given index in a List |

### List-SubLength

| Keys | Types | Help |
| --------- | --------- | --------- |
| LST | [List](List.html) |  |
| INDEX | [Integer](Integer.html) |  |
| NEWLEN | [Integer](Integer.html) |  |
| --- | --- | --- |
| Returns: | [List](List.html) |
| Help: | Sub-Length of a List |

