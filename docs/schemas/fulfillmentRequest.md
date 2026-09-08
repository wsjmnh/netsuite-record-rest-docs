# Schemas: fulfillmentRequest

Property tables for definitions owned by `fulfillmentRequest`.

Record page: [fulfillmentRequest](../records/fulfillmentRequest.md).

## Index

- [fulfillmentRequest](#fulfillmentrequest) — 34 properties
- [fulfillmentRequest-fulfillmentExceptionCollection](#fulfillmentrequest-fulfillmentexceptioncollection) — 6 properties
- [fulfillmentRequest-fulfillmentExceptionElement](#fulfillmentrequest-fulfillmentexceptionelement) — 10 properties
- [fulfillmentRequest-item-fulfillmentItemExceptionCollection](#fulfillmentrequest-item-fulfillmentitemexceptioncollection) — 6 properties
- [fulfillmentRequest-item-fulfillmentItemExceptionElement](#fulfillmentrequest-item-fulfillmentitemexceptionelement) — 9 properties
- [fulfillmentRequest-item-inventoryDetail](#fulfillmentrequest-item-inventorydetail) — 11 properties
- [fulfillmentRequest-item-inventoryDetail-inventoryAssignmentCollection](#fulfillmentrequest-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [fulfillmentRequest-item-inventoryDetail-inventoryAssignmentElement](#fulfillmentrequest-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [fulfillmentRequest-itemCollection](#fulfillmentrequest-itemcollection) — 6 properties
- [fulfillmentRequest-itemElement](#fulfillmentrequest-itemelement) — 46 properties
- [fulfillmentRequestCollection](#fulfillmentrequestcollection) — 6 properties
- [fulfillmentRequestSelectOptions](#fulfillmentrequestselectoptions) — 11 properties

## fulfillmentRequest

Browser definition `fulfillmentRequest`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assignee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | salesOrder |  |  | [`salesOrder`](salesOrder.md#salesorder) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fulfillmentException` |  | fulfillmentRequest-fulfillmentExceptionCollection |  |  | [`fulfillmentRequest-fulfillmentExceptionCollection`](#fulfillmentrequest-fulfillmentexceptioncollection) |  |
| `fulfillmentType` |  | object |  |  |  |  |
| `fulfillmentType.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `fulfillmentType.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isPickupEmailNotificationSent` | Pickup Email Notification Sent | boolean |  |  |  |  |
| `item` |  | fulfillmentRequest-itemCollection |  |  | [`fulfillmentRequest-itemCollection`](#fulfillmentrequest-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `orderId` | Order Id | string |  |  |  |  |
| `pickupHold` |  | object |  |  |  |  |
| `pickupHold.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `pickupHold.refName` | Reference Name | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `R`, `B`, `C`, `D`, `E`, `F`, `G`, `I` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Fulfillment Number | string |  |  |  |  |
| `tranStatus` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## fulfillmentRequest-fulfillmentExceptionCollection

Browser definition `fulfillmentRequest-fulfillmentExceptionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | fulfillmentRequest-fulfillmentExceptionElement[] |  |  | [`fulfillmentRequest-fulfillmentExceptionElement`](#fulfillmentrequest-fulfillmentexceptionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fulfillmentRequest-fulfillmentExceptionElement

Browser definition `fulfillmentRequest-fulfillmentExceptionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `exceptionComments` | Exception Comments | string |  |  |  |  |
| `exceptionQuantity` | Exception Quantity | number | float |  |  |  |
| `exceptionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `exceptionType` |  | object |  |  |  |  |
| `exceptionType.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `exceptionType.refName` | Reference Name | string |  |  |  |  |
| `itemLine` | Item | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantityRequested` | Quantity Requested | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## fulfillmentRequest-item-fulfillmentItemExceptionCollection

Browser definition `fulfillmentRequest-item-fulfillmentItemExceptionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | fulfillmentRequest-item-fulfillmentItemExceptionElement[] |  |  | [`fulfillmentRequest-item-fulfillmentItemExceptionElement`](#fulfillmentrequest-item-fulfillmentitemexceptionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fulfillmentRequest-item-fulfillmentItemExceptionElement

Browser definition `fulfillmentRequest-item-fulfillmentItemExceptionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `exceptionComments` | Exception Comments | string |  |  |  |  |
| `exceptionQuantity` | Exception Quantity | number | float |  |  |  |
| `exceptionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `exceptionType` |  | object |  |  |  |  |
| `exceptionType.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `exceptionType.refName` | Reference Name | string |  |  |  |  |
| `fulfillmentRequest` |  | fulfillmentRequest |  |  | [`fulfillmentRequest`](#fulfillmentrequest) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## fulfillmentRequest-item-inventoryDetail

Browser definition `fulfillmentRequest-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | fulfillmentRequest-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`fulfillmentRequest-item-inventoryDetail-inventoryAssignmentCollection`](#fulfillmentrequest-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## fulfillmentRequest-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `fulfillmentRequest-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | fulfillmentRequest-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`fulfillmentRequest-item-inventoryDetail-inventoryAssignmentElement`](#fulfillmentrequest-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fulfillmentRequest-item-inventoryDetail-inventoryAssignmentElement

Browser definition `fulfillmentRequest-item-inventoryDetail-inventoryAssignmentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `inventoryDetail` | Inventory Detail | integer | int64 |  |  |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `issueInventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packCarton` | Pack Carton | string |  |  |  |  |
| `pickCarton` | Pick Carton | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAvailable` | Unpicked Bin Qty | number | float |  |  |  |
| `receiptInventoryNumber` | Serial/Lot Number | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `toBinNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `toInventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |

## fulfillmentRequest-itemCollection

Browser definition `fulfillmentRequest-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | fulfillmentRequest-itemElement[] |  |  | [`fulfillmentRequest-itemElement`](#fulfillmentrequest-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fulfillmentRequest-itemElement

Browser definition `fulfillmentRequest-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `acknowledgeFulfillInstruction` | Acknowledge Instruction | boolean |  |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `currency` | Currency | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name | string |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `fulfillmentInstruction` |  | object |  |  |  |  |
| `fulfillmentInstruction.id` | Internal identifier | string |  |  |  | `F`, `N` |
| `fulfillmentInstruction.refName` | Reference Name | string |  |  |  |  |
| `fulfillmentItemException` |  | fulfillmentRequest-item-fulfillmentItemExceptionCollection |  |  | [`fulfillmentRequest-item-fulfillmentItemExceptionCollection`](#fulfillmentrequest-item-fulfillmentitemexceptioncollection) |  |
| `inventoryDetail` |  | fulfillmentRequest-item-inventoryDetail |  |  | [`fulfillmentRequest-item-inventoryDetail`](#fulfillmentrequest-item-inventorydetail) |  |
| `inventorysubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemFxAmount` | Foreign Amount | number | double |  |  |  |
| `itemName` | Item | string |  |  |  |  |
| `itemReceive` | Fulfill/Receive | boolean |  |  |  |  |
| `itemSubtype` | Subtype | string |  |  |  |  |
| `itemType` | Type | string |  |  |  |  |
| `itemUnitPrice` | Unit Price | number | double |  |  |  |
| `itemUpc` | UPC Code | string |  |  |  |  |
| `jobName` | Job | string |  |  |  |  |
| `kitMemberOf` | Member of Line | integer | int64 |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `lineEntity` | Entity | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `onHand` | On Hand | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `orderDoc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderLine` | Order Line | integer | int64 |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityPicked` | Picked | number | float |  |  |  |
| `quantityRemaining` | Quantity Remaining | number | float |  |  |  |
| `quantityRemainingDisplay` | Remaining | number | float |  |  |  |
| `quantityfulfilled` | Fulfilled | number | float |  |  |  |
| `quantitypacked` | Packed | number | float |  |  |  |
| `quantityrejected` | Quantity Rejected | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `requestNote` | Request Note | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `units` | Units | string |  |  |  |  |
| `unitsDisplay` | Units | string |  |  |  |  |

## fulfillmentRequestCollection

Browser definition `fulfillmentRequestCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | fulfillmentRequest[] |  |  | [`fulfillmentRequest`](#fulfillmentrequest) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fulfillmentRequestSelectOptions

Browser definition `fulfillmentRequestSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assignee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fulfillmentType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pickupHold` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `tranStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
