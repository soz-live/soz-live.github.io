
# Class:	String

| Fields | Values |
| --------- | --------- |
| Repo: | soz-live |
| Superclass: | [Atom](Atom.html) |
| Subclasses: | [PathName](PathName.html) <br> [SZMAClassName](SZMAClassName.html) <br> [SOZID](SOZID.html) <br> [AcDbHandle](AcDbHandle.html) <br> [String-Delim](String-Delim.html) <br> [Code](Code.html) <br> [Comment](Comment.html) <br> [Key](Key.html) <br> [Label](Label.html) |
| Interfaces: |  |
| Interfaced: | [SZLPString](SZLPString.html) |
| Abstract?: | No |
| isValue?: | Yes |
| Help: | String |

### String-Make

| Keys | Types |
| --------- | --------- |
| VALUE | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | New String Value |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [String->Integer](#String->Integer) <br> [String->Real](#String->Real) <br> [String->Strings](#String->Strings) <br> [String-AddToFront](#String-AddToFront) <br> [String-AddToRear](#String-AddToRear) <br> [String-CountChar](#String-CountChar) <br> [String-CountLeading](#String-CountLeading) <br> [String-Length](#String-Length) <br> [String-LowerCase](#String-LowerCase) <br> [String-PadFront](#String-PadFront) <br> [String-PadRear](#String-PadRear) <br> [String-RemoveChar](#String-RemoveChar) <br> [String-SwapDelim](#String-SwapDelim) <br> [String-UpperCase](#String-UpperCase) <br> [String-WCMatch](#String-WCMatch) |
| Super: | [Atom-Make](Atom.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### String->Integer

| Keys | Types |
| --------- | --------- |
| o | [String](String.html) |
| **---** | **---** |
| Returns: | [Integer](Integer.html) |
| Help: | String to Integer |

### String->Real

| Keys | Types |
| --------- | --------- |
| o | [String](String.html) |
| **---** | **---** |
| Returns: | [Real](Real.html) |
| Help: | String to Real |

### String->Strings

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| DELIM | [String](String.html) |
| **---** | **---** |
| Returns: | [Strings](Strings.html) |
| Help: | Convert String to Strings using Delim |

### String-AddToFront

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| NO | [Integer](Integer.html) |
| PAD | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | AddToFront of a String to a given Number |

### String-AddToRear

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| NO | [Integer](Integer.html) |
| PAD | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | AddToRear of a String to a given Number |

### String-CountChar

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| CHAR | [String](String.html) |
| **---** | **---** |
| Returns: | [Integer](Integer.html) |
| Help: | Number of characters matching in String |

### String-CountLeading

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| CHAR | [String](String.html) |
| **---** | **---** |
| Returns: | [Integer](Integer.html) |
| Help: | Number of leading characters matching |

### String-Length

| Keys | Types |
| --------- | --------- |
| o | [String](String.html) |
| **---** | **---** |
| Returns: | [Integer](Integer.html) |
| Help: | Length of a String |

### String-LowerCase

| Keys | Types |
| --------- | --------- |
| o | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | LowerCase String |

### String-PadFront

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| LEN | [Integer](Integer.html) |
| PAD | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | Pad the Front of a String to a given Length |

### String-PadRear

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| LEN | [Integer](Integer.html) |
| PAD | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | Pad the Rear of a String to a given Length |

### String-RemoveChar

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| CHAR | [String](String.html) |
| **---** | **---** |
| Returns: | [Integer](Integer.html) |
| Help: | Number of characters matching in String |

### String-SwapDelim

| Keys | Types |
| --------- | --------- |
| STR | [String](String.html) |
| FROM | [String](String.html) |
| TO | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | Swap Delim of a String |

### String-UpperCase

| Keys | Types |
| --------- | --------- |
| o | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | UpperCase String |

### String-WCMatch

| Keys | Types |
| --------- | --------- |
| o | [String](String.html) |
| pat | [String](String.html) |
| **---** | **---** |
| Returns: | [String](String.html) |
| Help: | WCMatch of a String |

