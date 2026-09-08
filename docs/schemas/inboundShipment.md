# Schemas: inboundShipment

Property tables for definitions owned by `inboundShipment`.

Record page: [inboundShipment](../records/inboundShipment.md).

## Index

- [inboundShipment](#inboundshipment) — 22 properties
- [inboundShipment-items-inventorydetail](#inboundshipment-items-inventorydetail) — 11 properties
- [inboundShipment-items-inventorydetail-inventoryAssignmentCollection](#inboundshipment-items-inventorydetail-inventoryassignmentcollection) — 6 properties
- [inboundShipment-items-inventorydetail-inventoryAssignmentElement](#inboundshipment-items-inventorydetail-inventoryassignmentelement) — 17 properties
- [inboundShipment-itemsCollection](#inboundshipment-itemscollection) — 6 properties
- [inboundShipment-itemsElement](#inboundshipment-itemselement) — 27 properties
- [inboundShipment-landedCostCollection](#inboundshipment-landedcostcollection) — 6 properties
- [inboundShipment-landedCostElement](#inboundshipment-landedcostelement) — 12 properties
- [inboundShipmentCollection](#inboundshipmentcollection) — 6 properties
- [inboundShipmentSelectOptions](#inboundshipmentselectoptions) — 3 properties

## inboundShipment

Browser definition `inboundShipment`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `actualDeliveryDate` | Actual Delivery Date | string | date |  |  |  |
| `actualShippingDate` | Actual Shipping Date | string | date |  |  |  |
| `billOfLading` | Bill Of Lading | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `expectedDeliveryDate` | Expected Delivery Date | string | date |  |  |  |
| `expectedShippingDate` | Expected Shipping Date | string | date |  |  |  |
| `externalDocumentNumber` | External Document Number | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `items` |  | inboundShipment-itemsCollection |  |  | [`inboundShipment-itemsCollection`](#inboundshipment-itemscollection) |  |
| `landedCost` |  | inboundShipment-landedCostCollection |  |  | [`inboundShipment-landedCostCollection`](#inboundshipment-landedcostcollection) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shipmentBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `shipmentCreatedDate` | Date Created | string | date |  |  |  |
| `shipmentMemo` | Memo | string |  |  |  |  |
| `shipmentNumber` | Shipment Number | string |  |  |  |  |
| `shipmentStatus` |  | object |  |  |  |  |
| `shipmentStatus.id` | Internal identifier | string |  |  |  | `toBeShipped`, `inTransit`, `partiallyReceived`, `received`, `closed` |
| `shipmentStatus.refName` | Reference Name | string |  |  |  |  |
| `vesselNumber` | Vessel Number | string |  |  |  |  |

## inboundShipment-items-inventorydetail

Browser definition `inboundShipment-items-inventorydetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | inboundShipment-items-inventorydetail-inventoryAssignmentCollection |  |  | [`inboundShipment-items-inventorydetail-inventoryAssignmentCollection`](#inboundshipment-items-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## inboundShipment-items-inventorydetail-inventoryAssignmentCollection

Browser definition `inboundShipment-items-inventorydetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inboundShipment-items-inventorydetail-inventoryAssignmentElement[] |  |  | [`inboundShipment-items-inventorydetail-inventoryAssignmentElement`](#inboundshipment-items-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inboundShipment-items-inventorydetail-inventoryAssignmentElement

Browser definition `inboundShipment-items-inventorydetail-inventoryAssignmentElement`.

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

## inboundShipment-itemsCollection

Browser definition `inboundShipment-itemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inboundShipment-itemsElement[] |  |  | [`inboundShipment-itemsElement`](#inboundshipment-itemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inboundShipment-itemsElement

Browser definition `inboundShipment-itemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocatedDemand` | Allocated Demand | string |  |  |  |  |
| `expectedRate` | Expected Rate | number | double |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `incoterm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `inventorydetail` |  | inboundShipment-items-inventorydetail |  |  | [`inboundShipment-items-inventorydetail`](#inboundshipment-items-inventorydetail) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `poCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `poRate` | PO Rate | number | double |  |  |  |
| `poVendor` | Vendor | string |  |  |  |  |
| `purchaseOrder` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `purchaseOrderTransaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `quantityBilled` | Quantity Billed | string |  |  |  |  |
| `quantityExpected` | Quantity Expected | string |  |  |  |  |
| `quantityReceived` | Quantity Received | string |  |  |  |  |
| `quantityRemaining` | Quantity Remaining | string |  |  |  |  |
| `receivingLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shipmentItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipmentItemAmount` | Amount | number | double |  |  |  |
| `shipmentItemDescription` | Description | string |  |  |  |  |
| `shipmentItemEffectiveDate` | Effective Date | string | date |  |  |  |
| `shipmentItemExchangeRate` | Exchange Rate | number | double |  |  |  |
| `shipmentItemTransaction` | PO Transaction Line | string |  |  |  |  |
| `totalUnitCost` | Total Unit Cost | number | double |  |  |  |
| `unit` | Unit | string |  |  |  |  |
| `unitLandedCost` | Unit Landed Cost | number | double |  |  |  |
| `vendorId` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |

## inboundShipment-landedCostCollection

Browser definition `inboundShipment-landedCostCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inboundShipment-landedCostElement[] |  |  | [`inboundShipment-landedCostElement`](#inboundshipment-landedcostelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inboundShipment-landedCostElement

Browser definition `inboundShipment-landedCostElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `landedCostAllocationMethod` |  | object |  |  |  |  |
| `landedCostAllocationMethod.id` | Internal identifier | string |  |  |  | `QUANTITY`, `VALUE`, `WEIGHT` |
| `landedCostAllocationMethod.refName` | Reference Name | string |  |  |  |  |
| `landedCostAmount` | Amount | number | double |  |  |  |
| `landedCostCostCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `landedCostCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `landedCostEffectiveDate` | Effective Date | string | date |  |  |  |
| `landedCostExchangeRate` | Exchange Rate | number | double |  |  |  |
| `landedCostId` | ID | integer | int64 |  |  |  |
| `landedCostShipmentItems` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## inboundShipmentCollection

Browser definition `inboundShipmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | inboundShipment[] |  |  | [`inboundShipment`](#inboundshipment) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inboundShipmentSelectOptions

Browser definition `inboundShipmentSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipmentBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipmentStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
