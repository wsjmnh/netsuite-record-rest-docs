# Schemas: bom

Property tables for definitions owned by `bom`.

Record page: [bom](../records/bom.md).

## Index

- [bom](#bom) — 20 properties
- [bom-assemblyCollection](#bom-assemblycollection) — 6 properties
- [bom-assemblyElement](#bom-assemblyelement) — 5 properties
- [bomCollection](#bomcollection) — 6 properties
- [bomSelectOptions](#bomselectoptions) — 5 properties

## bom

Browser definition `bom`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assembly` |  | bom-assemblyCollection |  |  | [`bom-assemblyCollection`](#bom-assemblycollection) |  |
| `availableForAllAssemblies` | Available For All Assemblies | boolean |  |  |  |  |
| `availableForAllLocations` | Available For All Locations | boolean |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `legacyBomForAssembly` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `restrictToAssemblies` |  | assemblyItemCollection |  |  | [`assemblyItemCollection`](assemblyItem.md#assemblyitemcollection) |  |
| `restrictToLocations` |  | locationCollection |  |  | [`locationCollection`](location.md#locationcollection) |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `useComponentYield` | Use Component Yield | boolean |  |  |  |  |
| `usedOnAssembly` | Used On Assembly | boolean |  |  |  |  |

## bom-assemblyCollection

Browser definition `bom-assemblyCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | bom-assemblyElement[] |  |  | [`bom-assemblyElement`](#bom-assemblyelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## bom-assemblyElement

Browser definition `bom-assemblyElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assembly` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `defaultForLocation` |  | locationCollection |  |  | [`locationCollection`](location.md#locationcollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `masterDefault` | Master Default | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## bomCollection

Browser definition `bomCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | bom[] |  |  | [`bom`](#bom) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## bomSelectOptions

Browser definition `bomSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `legacyBomForAssembly` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `restrictToAssemblies` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `restrictToLocations` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
