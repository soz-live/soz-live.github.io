
# Class:	File-TXT

### Description:

Text File



### Details:

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [File](File.html) |
| Subclasses: | [File-CSV](File-CSV.html) <br> [File-DAT](File-DAT.html) <br> [File-LSP](File-LSP.html) <br> [File-MD](File-MD.html) |
| Interfaces: |  |
| Interfaced: |  |
| Abstract?: | No |
| isValue?: | Yes |

### File-TXT-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| | | |
| Returns: |  | |
| Help: | |  |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [File-TXT-AppendLines](#File-TXT-AppendLines) <br> [File-TXT-Close](#File-TXT-Close) <br> [File-TXT-Open](#File-TXT-Open) <br> [File-TXT-ReadFirst](#File-TXT-ReadFirst) <br> [File-TXT-ReadLine](#File-TXT-ReadLine) <br> [File-TXT-ReadLines](#File-TXT-ReadLines) <br> [File-TXT-WriteLine](#File-TXT-WriteLine) <br> [File-TXT-WriteLines](#File-TXT-WriteLines) |
| Super: | [File-User_Select](File.html) <br> [File-User_Make](File.html) <br> [Atom-Make](Atom.html) <br> [T-Make](T.html) <br> [Logical-AND](Logical.html) <br> [Logical-OR](Logical.html) <br> [Logical-NOT](Logical.html) <br> [Logical-XOR](Logical.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### File-TXT-AppendLines

| Keys | Types | Help |
| --------- | --------- | --------- |
| FILENAME | [File-TXT](File-TXT.html) |  |
| LINES | [Strings](Strings.html) |  |
| | | |
| Returns: | [NIL](NIL.html) | |
| Help: | | Append Lines to a Text File |

### File-TXT-Close

| Keys | Types | Help |
| --------- | --------- | --------- |
| fn | [File-TXT](File-TXT.html) |  |
| | | |
| Returns: | [File-TXT](File-TXT.html) | |
| Help: | | Closing of a Text File |

### File-TXT-Open

| Keys | Types | Help |
| --------- | --------- | --------- |
| fn | [String](String.html) |  |
| access | [String](String.html) |  |
| | | |
| Returns: | [File-TXT](File-TXT.html) | |
| Help: | | Opening of a Text File |

### File-TXT-ReadFirst

| Keys | Types | Help |
| --------- | --------- | --------- |
| FILENAME | [File-TXT](File-TXT.html) |  |
| | | |
| Returns: | [Strings](Strings.html) | |
| Help: | | Reading First Line |

### File-TXT-ReadLine

| Keys | Types | Help |
| --------- | --------- | --------- |
| fn | [File-TXT](File-TXT.html) |  |
| | | |
| Returns: | [String](String.html) | |
| Help: | | Reading a line of a Text File |

### File-TXT-ReadLines

| Keys | Types | Help |
| --------- | --------- | --------- |
| FILENAME | [File-TXT](File-TXT.html) |  |
| | | |
| Returns: | [Strings](Strings.html) | |
| Help: | | Reading Text File Lines |

### File-TXT-WriteLine

| Keys | Types | Help |
| --------- | --------- | --------- |
| FILENAME | [File-TXT](File-TXT.html) |  |
| LINE | [String](String.html) |  |
| | | |
| Returns: | [File-TXT](File-TXT.html) | |
| Help: | | Writing a line to a Text File |

### File-TXT-WriteLines

| Keys | Types | Help |
| --------- | --------- | --------- |
| FILENAME | [File-TXT](File-TXT.html) |  |
| LINES | [Strings](Strings.html) |  |
| | | |
| Returns: | [NIL](NIL.html) | |
| Help: | | Writing lines to a Text File |

