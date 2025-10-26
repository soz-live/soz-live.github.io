
# Class:	AcDbDocument

## Description:

Base Document Class


| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [AcDbObject](AcDbObject.html) |
| Subclasses: |  |
| Interfaces: |  |
| Interfaced: |  |
| Abstract?: | Yes |
| isValue?: | No |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDbDocument-ActiveSpace](#AcDbDocument-ActiveSpace) <br> [AcDbDocument-AddCustomInfoByKey](#AcDbDocument-AddCustomInfoByKey) <br> [AcDbDocument-GetAllCustomInfo](#AcDbDocument-GetAllCustomInfo) <br> [AcDbDocument-SetAllCustomInfo](#AcDbDocument-SetAllCustomInfo) <br> [AcDbDocument-SetCustomInfoByKey](#AcDbDocument-SetCustomInfoByKey) |
| Super: | [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDbDocument-ActiveSpace

| Keys | Types | Help |
| --------- | --------- | --------- |
| O | [AcDbDocument](AcDbDocument.html) |  |
| --- | --- | --- |
| Returns: | [AcDbBlock](AcDbBlock.html) |
| Help: | ActiveSpace of an AcDbDocument |

### AcDbDocument-AddCustomInfoByKey

| Keys | Types | Help |
| --------- | --------- | --------- |
| DOC | [AcDbDocument](AcDbDocument.html) |  |
| KEY | [Key](Key.html) |  |
| VALUE | [Comment](Comment.html) |  |
| --- | --- | --- |
| Returns: | [AcDbCustomInfo](AcDbCustomInfo.html) |
| Help: | Add CustomInfo |

### AcDbDocument-GetAllCustomInfo

| Keys | Types | Help |
| --------- | --------- | --------- |
| DOC | [AcDbDocument](AcDbDocument.html) |  |
| --- | --- | --- |
| Returns: | [Structure](Structure.html) |
| Help: | Get All CustomInfo |

### AcDbDocument-SetAllCustomInfo

| Keys | Types | Help |
| --------- | --------- | --------- |
| DOC | [AcDbDocument](AcDbDocument.html) |  |
| AL | [Structure](Structure.html) |  |
| --- | --- | --- |
| Returns: | [Structure](Structure.html) |
| Help: | Set CustomInfo |

### AcDbDocument-SetCustomInfoByKey

| Keys | Types | Help |
| --------- | --------- | --------- |
| DOC | [AcDbDocument](AcDbDocument.html) |  |
| KEY | [Key](Key.html) |  |
| VALUE | [Comment](Comment.html) |  |
| --- | --- | --- |
| Returns: | [NIL](NIL.html) |
| Help: | Set CustomInfo Key |

