# Schemas: manufacturingRouting

Property tables for definitions owned by `manufacturingRouting`.

Record page: [manufacturingRouting](../records/manufacturingRouting.md).

## Index

- [manufacturingRouting](#manufacturingrouting) — 16 properties
- [manufacturingRouting-routingComponentCollection](#manufacturingrouting-routingcomponentcollection) — 6 properties
- [manufacturingRouting-routingComponentElement](#manufacturingrouting-routingcomponentelement) — 12 properties
- [manufacturingRouting-routingStepCollection](#manufacturingrouting-routingstepcollection) — 6 properties
- [manufacturingRouting-routingStepElement](#manufacturingrouting-routingstepelement) — 19 properties
- [manufacturingRoutingCollection](#manufacturingroutingcollection) — 6 properties
- [manufacturingRoutingSelectOptions](#manufacturingroutingselectoptions) — 5 properties

## manufacturingRouting

Browser definition `manufacturingRouting`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `autoCalculateLag` | Auto-calculate Lag | boolean |  |  |  |  |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isDefault` | Default | boolean |  |  |  |  |
| `isInactive` | Is Inactive | boolean |  |  |  |  |
| `item` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | locationCollection |  |  | [`locationCollection`](location.md#locationcollection) |  |
| `memo` | Memo | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `routingComponent` |  | manufacturingRouting-routingComponentCollection |  |  | [`manufacturingRouting-routingComponentCollection`](#manufacturingrouting-routingcomponentcollection) |  |
| `routingStep` |  | manufacturingRouting-routingStepCollection |  |  | [`manufacturingRouting-routingStepCollection`](#manufacturingrouting-routingstepcollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## manufacturingRouting-routingComponentCollection

Browser definition `manufacturingRouting-routingComponentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | manufacturingRouting-routingComponentElement[] |  |  | [`manufacturingRouting-routingComponentElement`](#manufacturingrouting-routingcomponentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingRouting-routingComponentElement

Browser definition `manufacturingRouting-routingComponentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `bomQuantity` | BoM Quantity | number | float |  |  |  |
| `component` | Component | string |  |  |  |  |
| `description` | Description | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lineNumber` | Line Number | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `operationSequenceNumber` | Operation Sequence | integer | int64 |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `units` | Units | string |  |  |  |  |
| `yield` | Yield | number | double |  |  |  |

## manufacturingRouting-routingStepCollection

Browser definition `manufacturingRouting-routingStepCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | manufacturingRouting-routingStepElement[] |  |  | [`manufacturingRouting-routingStepElement`](#manufacturingrouting-routingstepelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingRouting-routingStepElement

Browser definition `manufacturingRouting-routingStepElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `connectionType` |  | object |  |  |  |  |
| `connectionType.id` | Internal identifier | string |  |  |  | `FS`, `SS` |
| `connectionType.refName` | Reference Name | string |  |  |  |  |
| `laborResources` | Labor Resources | number | float |  |  |  |
| `lagAmount` | Lag Amount | integer | int64 |  |  |  |
| `lagType` |  | object |  |  |  |  |
| `lagType.id` | Internal identifier | string |  |  |  | `quantity`, `timepercent`, `time`, `qtypercent` |
| `lagType.refName` | Reference Name | string |  |  |  |  |
| `lagUnits` | Lag Units | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `machineResources` | Machine Resources | number | float |  |  |  |
| `manufacturingCostTemplate` |  | manufacturingCostTemplate |  |  | [`manufacturingCostTemplate`](manufacturingCostTemplate.md#manufacturingcosttemplate) |  |
| `manufacturingWorkCenter` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `operationName` | Operation Name | string |  |  |  |  |
| `operationSequence` | Operation Sequence | integer | int64 |  |  |  |
| `operationYield` | Operation Yield | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `runRate` | Run Rate (Min/Unit) | number | float |  |  |  |
| `setupTime` | Setup Time (Min) | number | float |  |  |  |

## manufacturingRoutingCollection

Browser definition `manufacturingRoutingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | manufacturingRouting[] |  |  | [`manufacturingRouting`](#manufacturingrouting) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## manufacturingRoutingSelectOptions

Browser definition `manufacturingRoutingSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
