
# Class:	String

### Description:

String



### Details:

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [Atom](Atom.html) |
| Subclasses: | [Documentation](Documentation.html) <br> [Date](Date.html) <br> [Second](Second.html) <br> [Minute](Minute.html) <br> [Hour](Hour.html) <br> [Day](Day.html) <br> [Month](Month.html) <br> [Year](Year.html) <br> [PathName](PathName.html) <br> [SZMAClassName](SZMAClassName.html) <br> [SOZID](SOZID.html) <br> [AcDbHandle](AcDbHandle.html) <br> [String-Delim](String-Delim.html) <br> [Code](Code.html) <br> [Comment](Comment.html) <br> [Key](Key.html) <br> [Label](Label.html) |
| Interfaces: |  |
| Interfaced: | [SZLPString](SZLPString.html) |
| Abstract?: | No |
| isValue?: | Yes |

### String-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| VALUE | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | New String Value |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [String->Integer](#String->Integer) <br> [String->Real](#String->Real) <br> [String->Strings](#String->Strings) <br> [String-AddToFront](#String-AddToFront) <br> [String-AddToRear](#String-AddToRear) <br> [String-CountAscii](#String-CountAscii) <br> [String-CountChar](#String-CountChar) <br> [String-CountLeading](#String-CountLeading) <br> [String-FindPosition](#String-FindPosition) <br> [String-Length](#String-Length) <br> [String-LowerCase](#String-LowerCase) <br> [String-PadFront](#String-PadFront) <br> [String-PadRear](#String-PadRear) <br> [String-RemoveChar](#String-RemoveChar) <br> [String-SwapDelim](#String-SwapDelim) <br> [String-UpperCase](#String-UpperCase) <br> [String-WCMatch](#String-WCMatch) |
| Super: | [Atom-Make](Atom.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### String->Integer

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [String](String.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | String to Integer |

### String->Real

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [String](String.html) |  |
| | | |
| Returns: | [Real](Real.html) | |
| Help: | | String to Real |

### String->Strings

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| DELIM | [String](String.html) |  |
| | | |
| Returns: | [Strings](Strings.html) | |
| Help: | | Convert String to Strings using Delim |

### String-AddToFront

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| NO | [Integer](Integer.html) |  |
| PAD | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | AddToFront of a String to a given Number |

### String-AddToRear

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| NO | [Integer](Integer.html) |  |
| PAD | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | AddToRear of a String to a given Number |

### String-CountAscii

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| CHAR | [Integer](Integer.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | Number of Ascii Char matching in String |

### String-CountChar

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| CHAR | [String](String.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | Number of characters matching in String |

### String-CountLeading

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| CHAR | [String](String.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | Number of leading characters matching |

### String-FindPosition

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| CHAR | [Integer](Integer.html) |  |
| POSN | [Integer](Integer.html) |  |
| END | [Boolean](Boolean.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | Position in String of char |

### String-Length

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [String](String.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | Length of a String |

### String-LowerCase

| Keys | Types | Help |
| --------- | --------- | --------- |
| o | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | LowerCase String |

### String-PadFront

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| LEN | [Integer](Integer.html) |  |
| PAD | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | Pad the Front of a String to a given Length |

### String-PadRear

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| LEN | [Integer](Integer.html) |  |
| PAD | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | Pad the Rear of a String to a given Length |

### String-RemoveChar

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| CHAR | [String](String.html) |  |
| | | |
| Returns: | [Integer](Integer.html) | |
| Help: | | Number of characters matching in String |

### String-SwapDelim

| Keys | Types | Help |
| --------- | --------- | --------- |
| STR | [String](String.html) |  |
| FROM | [String](String.html) |  |
| TO | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | Swap Delim of a String |

### String-UpperCase

| Keys | Types | Help |
| --------- | --------- | --------- |
| o | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | UpperCase String |

### String-WCMatch

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [String](String.html) |  |
| PAT | [String](String.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | WCMatch of a String |

