# Schemas: itemSupplyPlan

Property tables for definitions owned by `itemSupplyPlan`.

Record page: [itemSupplyPlan](../records/itemSupplyPlan.md).

## Index

- [itemSupplyPlan](#itemsupplyplan) — 13 properties
- [itemSupplyPlan-orderCollection](#itemsupplyplan-ordercollection) — 6 properties
- [itemSupplyPlan-orderElement](#itemsupplyplan-orderelement) — 9 properties
- [itemSupplyPlan-planningmessageCollection](#itemsupplyplan-planningmessagecollection) — 6 properties
- [itemSupplyPlan-planningmessageElement](#itemsupplyplan-planningmessageelement) — 11 properties
- [itemSupplyPlanCollection](#itemsupplyplancollection) — 6 properties
- [itemSupplyPlanSelectOptions](#itemsupplyplanselectoptions) — 5 properties

## itemSupplyPlan

Browser definition `itemSupplyPlan`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `order` |  | itemSupplyPlan-orderCollection |  |  | [`itemSupplyPlan-orderCollection`](#itemsupplyplan-ordercollection) |  |
| `planningmessage` |  | itemSupplyPlan-planningmessageCollection |  |  | [`itemSupplyPlan-planningmessageCollection`](#itemsupplyplan-planningmessagecollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `units` | Unit of Measure | string |  |  |  |  |

## itemSupplyPlan-orderCollection

Browser definition `itemSupplyPlan-orderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemSupplyPlan-orderElement[] |  |  | [`itemSupplyPlan-orderElement`](#itemsupplyplan-orderelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemSupplyPlan-orderElement

Browser definition `itemSupplyPlan-orderElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `orderdate` | Order Date | string | date |  |  |  |
| `orderdockey` | Order Id | integer | int64 |  |  |  |
| `ordertype` |  | object |  |  |  |  |
| `ordertype.id` | Internal identifier | string |  |  |  | `VendPymt`, `STaxLiab`, `CustCred`, `ItemShip`, `Check`, `RevContr`, `CustChrg`, `Journal`, `OrdResv`, `RevArrng`, `GLAdj`, `InvReval`, `Opprtnty`, `CustRfnd`, `TrnfrOrd`, `CashRfnd`, `Build`, `Unbuild`, `RevComm`, `SalesOrd`, `Rfq`, `VPrepApp`, `TegPybl`, `Deposit`, `WOIssue`, `FinChrg`, `PurchOrd`, `FftReq`, `StatChng`, `DepAppl`, `ExpRept`, `Wave`, `OwnTrnsf`, `StPickUp`, `NettStlm`, `TegRcvbl`, `WOCompl`, `InvAdjst`, `Transfer`, `Paycheck`, `BalJrnal`, `VendBill`, `YtdAdjst`, `XChgJrnl`, `ItemRcpt`, `PChkJrnl`, `Estimate`, `VPrep`, `SysJrnl`, `Commissn`, `TaxPymt`, `RtnAuth`, `CustInvc`, `WorkOrd`, `FxReval`, `PurchCon`, `BinTrnfr`, `LiaAdjst`, `InvDistr`, `LiabPymt`, `VendRfq`, `RevComRv`, `TaxLiab`, `InvcGrp`, `CustAuth`, `VendAuth`, `InvCount`, `CardRfnd`, `InvWksht`, `VendCred`, `PEJrnl`, `BinWksht`, `Custom`, `CustDep`, `CustPymt`, `WOClose`, `PurchReq`, `InbShip`, `CashSale`, `BlankOrd`, `DeprCust`, `CardChrg`, `InvTrnfr` |
| `ordertype.refName` | Reference Name | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `receiptdate` | Receipt Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemSupplyPlan-planningmessageCollection

Browser definition `itemSupplyPlan-planningmessageCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemSupplyPlan-planningmessageElement[] |  |  | [`itemSupplyPlan-planningmessageElement`](#itemsupplyplan-planningmessageelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemSupplyPlan-planningmessageElement

Browser definition `itemSupplyPlan-planningmessageElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `creationdate` | Date Created | string | date |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Message | string |  |  |  |  |
| `messagecode` | Message Code | integer | int64 |  |  |  |
| `orderurl` | URL | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `receiptdate` | Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `rescheduledate` | Reschedule Date | string | date |  |  |  |
| `transactionid` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `transactionlineid` | Order Line | string |  |  |  |  |

## itemSupplyPlanCollection

Browser definition `itemSupplyPlanCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | itemSupplyPlan[] |  |  | [`itemSupplyPlan`](#itemsupplyplan) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemSupplyPlanSelectOptions

Browser definition `itemSupplyPlanSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
