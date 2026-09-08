# Schemas: entityGroup

Property tables for definitions owned by `entityGroup`.

Record page: [entityGroup](../records/entityGroup.md).

## Index

- [entityGroup](#entitygroup) — 30 properties
- [entityGroup-groupMembersCollection](#entitygroup-groupmemberscollection) — 6 properties
- [entityGroup-groupMembersElement](#entitygroup-groupmemberselement) — 26 properties
- [entityGroup-testCellCollection](#entitygroup-testcellcollection) — 6 properties
- [entityGroup-testCellElement](#entitygroup-testcellelement) — 5 properties
- [entityGroupCollection](#entitygroupcollection) — 6 properties
- [entityGroupSelectOptions](#entitygroupselectoptions) — 7 properties

## entityGroup

Browser definition `entityGroup`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `comments` | Comments | string |  |  |  |  |
| `email` | Email | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `groupMembers` |  | entityGroup-groupMembersCollection |  |  | [`entityGroup-groupMembersCollection`](#entitygroup-groupmemberscollection) |  |
| `groupMembership` | Membership | string |  |  |  |  |
| `groupName` | Name | string |  |  |  |  |
| `groupOwner` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `groupType` |  | object |  |  |  |  |
| `groupType.id` | Internal identifier | string |  |  |  | `Employee`, `CustJob`, `Vendor`, `Job`, `Partner`, `Contact` |
| `groupType.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isFunctionalTeam` | Functional Team | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isManufacturingWorkCenter` | Manufacturing Work Center | boolean |  |  |  |  |
| `isPrivate` | Private | boolean |  |  |  |  |
| `isProductTeam` | Product Team | boolean |  |  |  |  |
| `isSalesRep` | Sales Group | boolean |  |  |  |  |
| `isSupportRep` | Support Group | boolean |  |  |  |  |
| `issueRole` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `laborResources` | Labor Resources | number | float |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `machineResources` | Machine Resources | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `restrictedToOwner` | Restrict Group Editing to Owner | boolean |  |  |  |  |
| `restrictionGroup` |  | entityGroup |  |  | [`entityGroup`](#entitygroup) |  |
| `savedSearch` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `size` | Size | integer | int64 |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `testCell` |  | entityGroup-testCellCollection |  |  | [`entityGroup-testCellCollection`](#entitygroup-testcellcollection) |  |
| `workCalendar` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## entityGroup-groupMembersCollection

Browser definition `entityGroup-groupMembersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | entityGroup-groupMembersElement[] |  |  | [`entityGroup-groupMembersElement`](#entitygroup-groupmemberselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## entityGroup-groupMembersElement

Browser definition `entityGroup-groupMembersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessLevel` |  | object |  |  |  |  |
| `accessLevel.id` | Internal identifier | string |  |  |  | `0`, `1`, `2`, `3`, `4` |
| `accessLevel.refName` | Reference Name | string |  |  |  |  |
| `bouncedAddress` | Bounced | boolean |  |  |  |  |
| `company` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `contactMember` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contribution` | Contribution % | number | double |  |  |  |
| `custJobMember` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `email` | Email | string |  |  |  |  |
| `employeeMember` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `isSalesRep` | Is Sales Representative | boolean |  |  |  |  |
| `jobMember` |  | job |  |  | [`job`](job.md#job) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `member` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `name` | Name | string |  |  |  |  |
| `partnerMember` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `phone` | Phone | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salesRep` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `salesRole` |  | salesRole |  |  | [`salesRole`](salesRole.md#salesrole) |  |
| `subscriptionStatus` |  | object |  |  |  |  |
| `subscriptionStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `subscriptionStatus.refName` | Reference Name | string |  |  |  |  |
| `vendorMember` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |

## entityGroup-testCellCollection

Browser definition `entityGroup-testCellCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | entityGroup-testCellElement[] |  |  | [`entityGroup-testCellElement`](#entitygroup-testcellelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## entityGroup-testCellElement

Browser definition `entityGroup-testCellElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cellId` | ID | integer | int64 |  |  |  |
| `cellName` | Name | string |  |  |  |  |
| `cellPercent` | Percentage | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## entityGroupCollection

Browser definition `entityGroupCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | entityGroup[] |  |  | [`entityGroup`](#entitygroup) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## entityGroupSelectOptions

Browser definition `entityGroupSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `groupOwner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `groupType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueRole` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `restrictionGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `savedSearch` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `workCalendar` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
