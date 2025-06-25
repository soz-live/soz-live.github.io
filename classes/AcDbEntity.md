
# Class:	AcDbEntity

| Fields | Values |
| --------- | --------- |
| Repo: | [soz-live](/repos/soz-live.html) |
| Superclass: | [AcDbObject](AcDbObject.html) |
| Subclasses: | [BsysEntity](BsysEntity.html) <br> [SZCELinear](SZCELinear.html) <br> [SZCEPlane](SZCEPlane.html) <br> [ACISEntity](ACISEntity.html) <br> [AcDbCurve](AcDbCurve.html) <br> [AcDbViewport](AcDbViewport.html) <br> [AcDbRay](AcDbRay.html) <br> [AcDbXline](AcDbXline.html) <br> [AcDbPoint](AcDbPoint.html) <br> [AcDbAbstractText](AcDbAbstractText.html) <br> [AcDbAttributeDefinition](AcDbAttributeDefinition.html) <br> [AcDbBlockReference](AcDbBlockReference.html) <br> [AcDbFace](AcDbFace.html) <br> [AcDbMesh](AcDbMesh.html) |
| Interfaces: |  |
| Interfaced: |  |
| Abstract?: | Yes |
| isValue?: | No |
| Help: | Base Entity Class |


## Functions:

| Types | Functions |
| --------- | --------- |
| Class: | [AcDbEntity-Copy](#AcDbEntity-Copy) <br> [AcDbEntity-ExternalCopy](#AcDbEntity-ExternalCopy) <br> [AcDbEntity-Highlight](#AcDbEntity-Highlight) <br> [AcDbEntity-InternalCopy](#AcDbEntity-InternalCopy) <br> [AcDbEntity-IntersectWith](#AcDbEntity-IntersectWith) <br> [AcDbEntity-Layer](#AcDbEntity-Layer) <br> [AcDbEntity-Move](#AcDbEntity-Move) <br> [AcDbEntity-SZCOColor](#AcDbEntity-SZCOColor) <br> [AcDbEntity-SetVisibility](#AcDbEntity-SetVisibility) <br> [AcDbEntity-SetVisual](#AcDbEntity-SetVisual) <br> [AcDbEntity-Space](#AcDbEntity-Space) <br> [AcDbEntity-Transformby](#AcDbEntity-Transformby) <br> [AcDbEntity-User_Pick](#AcDbEntity-User_Pick) <br> [AcDbEntity-User_PickList](#AcDbEntity-User_PickList) <br> [AcDbEntity-User_PickModel](#AcDbEntity-User_PickModel) <br> [AcDbEntity-User_PickNode](#AcDbEntity-User_PickNode) <br> [AcDbEntity-User_PickSet](#AcDbEntity-User_PickSet) <br> [AcDbEntity-Visual](#AcDbEntity-Visual) |
| Super: | [SZOBObject->SOZFile](SZOBObject.html) <br> [SZOBBase-User_Select](SZOBBase.html) <br> [SZOBBase-User_Make](SZOBBase.html) <br> [SZOBBase-User_Method](SZOBBase.html) <br> [SZOBBase-User_ObjectKey](SZOBBase.html) <br> [SZOBBase-User_Edit](SZOBBase.html) <br> [SZOBBase-User_Clone](SZOBBase.html) <br> [SZOBBase-User_PickNode](SZOBBase.html) <br> [SZOBBase-User_PickModel](SZOBBase.html) |


### AcDbEntity-Copy

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Copy Entity |

### AcDbEntity-ExternalCopy

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| PARENT | [AcDbBlockReference](AcDbBlockReference.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | External Copy of an Entitiy |

### AcDbEntity-Highlight

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| BOOL | [Boolean](Boolean.html) |  |
| --- | --- | --- |
| Returns: | [Boolean](Boolean.html) |
| Help: | Set Entities Highlight |

### AcDbEntity-InternalCopy

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| PARENT | [SZCEModelRef](SZCEModelRef.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Internal Copy of an Entitiy |

### AcDbEntity-IntersectWith

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY0 | [AcDbEntity](AcDbEntity.html) |  |
| ENTITY1 | [AcDbEntity](AcDbEntity.html) |  |
| EXTEND | [Enum-AcDbExtend](Enum-AcDbExtend.html) |  |
| --- | --- | --- |
| Returns: | [Points](Points.html) |
| Help: | IntersectWith |

### AcDbEntity-Layer

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [AcDbLayerTableRecord](AcDbLayerTableRecord.html) |
| Help: | get Entities's Layer |

### AcDbEntity-Move

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| POINT0 | [SZGEPoint](SZGEPoint.html) |  |
| POINT1 | [SZGEPoint](SZGEPoint.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Move Entity from Point to Point |

### AcDbEntity-SZCOColor

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [SZCOColor](SZCOColor.html) |
| Help: | get Entities's TrueColor |

### AcDbEntity-SetVisibility

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| VIS | [Boolean](Boolean.html) |  |
| --- | --- | --- |
| Returns: | [Boolean](Boolean.html) |
| Help: | Set Entities Visibility |

### AcDbEntity-SetVisual

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| VISUAL | [SZCOVisual](SZCOVisual.html) | Visual Settings |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Sets the Visual Settings for the Entity |

### AcDbEntity-Space

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [AcDbBlock](AcDbBlock.html) |
| Help: | get Entities's Space |

### AcDbEntity-Transformby

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| TMATRIX | [SZGETMatrix](SZGETMatrix.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Transform Entity by TMatrix |

### AcDbEntity-User_Pick

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | User_Pick |

### AcDbEntity-User_PickList

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [List:AcDbEntity](AcDbEntity.html) |
| Help: | User_PickList |

### AcDbEntity-User_PickModel

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | User_PickModel |

### AcDbEntity-User_PickNode

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | User_PickNode |

### AcDbEntity-User_PickSet

| Keys | Types | Help |
| --------- | --------- | --------- |
| USER | [User](User.html) |  |
| --- | --- | --- |
| Returns: | [Set:AcDbEntity](AcDbEntity.html) |
| Help: | User_PickSet |

### AcDbEntity-Visual

| Keys | Types | Help |
| --------- | --------- | --------- |
| ENTITY | [AcDbEntity](AcDbEntity.html) |  |
| --- | --- | --- |
| Returns: | [AcDbEntity](AcDbEntity.html) |
| Help: | Gets the Visual Settings for the Entity |

