
# Class:	SZCOVisual

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [SZCOObject](SZCOObject.html) |
| Subclasses: | [SZCOVisual-Entity](SZCOVisual-Entity.html) <br> [SZCOVisual-Current](SZCOVisual-Current.html) <br> [SZCOVisual-Default](SZCOVisual-Default.html) <br> [SZCOVisual-Color](SZCOVisual-Color.html) <br> [SZCOVisual-ByLayer](SZCOVisual-ByLayer.html) |
| Interfaces: |  |
| Interfaced: |  |
| Abstract?: | No |
| isValue?: | No |
| Help: | SZCOVisual |

### SZCOVisual-Make

| Keys | Types | Help |
| --------- | --------- | --------- |
| LAYER | [AcDbLayerTableRecord](AcDbLayerTableRecord.html) |  |
| COLOR | [SZCOColor](SZCOColor.html) |  |
| LTYPE | [AcDbLineType](AcDbLineType.html) |  |
| LWEIGHT | [Enum-AcDbLineWeight](Enum-AcDbLineWeight.html) |  |
| --- | --- | --- |
| Returns: | [SZCOVisual](SZCOVisual.html) |
| Help: | SZCOVisual |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [SZCOVisual-SetEntities](#SZCOVisual-SetEntities) <br> [SZCOVisual-SetEntity](#SZCOVisual-SetEntity) |
| Super: | [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### SZCOVisual-SetEntities

| Keys | Types | Help |
| --------- | --------- | --------- |
| VIZ | [SZCOVisual](SZCOVisual.html) | Visual Settings |
| ENTS | [Set:AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [Set:AcDbEntity](AcDbEntity.html) |
| Help: | Sets the Visual Settings for the Entity |

### SZCOVisual-SetEntity

| Keys | Types | Help |
| --------- | --------- | --------- |
| VIZ | [SZCOVisual](SZCOVisual.html) | Visual Settings |
| ENT | [AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Sets the Visual Settings for the Entity |

