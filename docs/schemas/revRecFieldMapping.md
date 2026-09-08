# Schemas: revRecFieldMapping

Property tables for definitions owned by `revRecFieldMapping`.

Record page: [revRecFieldMapping](../records/revRecFieldMapping.md).

## Index

- [revRecFieldMapping](#revrecfieldmapping) — 17 properties
- [revRecFieldMappingCollection](#revrecfieldmappingcollection) — 6 properties
- [revRecFieldMappingSelectOptions](#revrecfieldmappingselectoptions) — 5 properties

## revRecFieldMapping

Browser definition `revRecFieldMapping`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `autoupdatetargetfieldvalue` | Automatically Update Target Field Value | boolean |  |  |  |  |
| `customtxform` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `enddate` | End Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sourcefield` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `sourcerecordtype` |  | object |  |  |  |  |
| `sourcerecordtype.id` | Internal identifier | string |  |  |  | `TRANSACTION_LINE` |
| `sourcerecordtype.refName` | Reference Name | string |  |  |  |  |
| `startdate` | Start Date | string | date |  |  |  |
| `targetfield` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `transactiontype` |  | object |  |  |  |  |
| `transactiontype.id` | Internal identifier | string |  |  |  | `VendPymt`, `CustCred`, `ItemShip`, `Check`, `Journal`, `CustChrg`, `Opprtnty`, `CustRfnd`, `CashRfnd`, `TrnfrOrd`, `Build`, `Unbuild`, `RevComm`, `SalesOrd`, `TegPybl`, `Deposit`, `WOIssue`, `FinChrg`, `PurchOrd`, `ExpRept`, `DepAppl`, `TegRcvbl`, `WOCompl`, `InvAdjst`, `Transfer`, `Paycheck`, `YtdAdjst`, `VendBill`, `ItemRcpt`, `Estimate`, `PChkJrnl`, `SysJrnl`, `Commissn`, `TaxPymt`, `RtnAuth`, `CustInvc`, `FxReval`, `WorkOrd`, `BinTrnfr`, `LiaAdjst`, `InvDistr`, `LiabPymt`, `RevComRv`, `CuTrPrch`, `VendAuth`, `InvWksht`, `CardRfnd`, `VendCred`, `BinWksht`, `Custom`, `CustPymt`, `CustDep`, `WOClose`, `CashSale`, `CuTrSale`, `DeprCust`, `CardChrg`, `InvTrnfr` |
| `transactiontype.refName` | Reference Name | string |  |  |  |  |

## revRecFieldMappingCollection

Browser definition `revRecFieldMappingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | revRecFieldMapping[] |  |  | [`revRecFieldMapping`](#revrecfieldmapping) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## revRecFieldMappingSelectOptions

Browser definition `revRecFieldMappingSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customtxform` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourcefield` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourcerecordtype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `targetfield` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactiontype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
