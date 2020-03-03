# CreditRefillSOS

Name: **CreditRefillSOS**
Description: **for analysis - DONT USE THIS VERSION**
Type: **Sales**
SubType: **CreditRefillSOS**

---

### GetUserType (DataRaptor Extract Action)

* El DataRaptor recibe como parámetro el elemento `userId`.
* Crea un nodo `userType` relleno con el campo `UserType` del `User` a partir del

### InitData (Set Values)

Element Value Map:

| Element Name | Value |
| ----------- | ----------- |
| `ContextId` | %`ContextId`% |
| `ProductCode` | FAN_PA_SOS_00001 |

### InitData1 (Set Values)

##### Element Value Map
| Element Name | Value |
| ----------- | ----------- |
| `Id` | %`ContextId`% |

### ta-sales-getAssetInfoById (DataRaptor Extract Action)

* El DataRaptor recibe como parámetro el elemento `ContextId`.
* Devuelve un nodo `Asset` relleno con varios campos con información de dicho elemento.

### SetAssetInfo (Set Values)

##### Element Value Map
| Element Name | Value |
| ----------- | ----------- |
| `accountId` | %`Asset:AccountId`% |
| `lineNumber` | %`Asset:LineNumber`% |

### S439_QueryLite_CBS (Integration Procedure Action)
* Integration Procedure: **IFS_S439**
