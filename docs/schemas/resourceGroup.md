# Schemas: resourceGroup

Property tables for definitions owned by `resourceGroup`.

Record page: [resourceGroup](../records/resourceGroup.md).

## Index

- [resourceGroup](#resourcegroup) — 9 properties
- [resourceGroup-resourceGroupMembersCollection](#resourcegroup-resourcegroupmemberscollection) — 6 properties
- [resourceGroup-resourceGroupMembersElement](#resourcegroup-resourcegroupmemberselement) — 3 properties
- [resourceGroupCollection](#resourcegroupcollection) — 6 properties
- [resourceGroupSelectOptions](#resourcegroupselectoptions) — 1 properties

## resourceGroup

Browser definition `resourceGroup`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `resourceGroupMembers` |  | resourceGroup-resourceGroupMembersCollection |  |  | [`resourceGroup-resourceGroupMembersCollection`](#resourcegroup-resourcegroupmemberscollection) |  |

## resourceGroup-resourceGroupMembersCollection

Browser definition `resourceGroup-resourceGroupMembersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | resourceGroup-resourceGroupMembersElement[] |  |  | [`resourceGroup-resourceGroupMembersElement`](#resourcegroup-resourcegroupmemberselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## resourceGroup-resourceGroupMembersElement

Browser definition `resourceGroup-resourceGroupMembersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `resource` |  | employee |  |  | [`employee`](employee.md#employee) |  |

## resourceGroupCollection

Browser definition `resourceGroupCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | resourceGroup[] |  |  | [`resourceGroup`](#resourcegroup) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## resourceGroupSelectOptions

Browser definition `resourceGroupSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
