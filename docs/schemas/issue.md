# Schemas: issue

Property tables for definitions owned by `issue`.

Record page: [issue](../records/issue.md).

## Index

- [issue](#issue) — 55 properties
- [issue-brokenInVersionCollection](#issue-brokeninversioncollection) — 6 properties
- [issue-brokenInVersionElement](#issue-brokeninversionelement) — 5 properties
- [issue-fixedInVersionCollection](#issue-fixedinversioncollection) — 6 properties
- [issue-fixedInVersionElement](#issue-fixedinversionelement) — 5 properties
- [issue-relatedIssuesCollection](#issue-relatedissuescollection) — 6 properties
- [issue-relatedIssuesElement](#issue-relatedissueselement) — 11 properties
- [issue-targetVersionCollection](#issue-targetversioncollection) — 6 properties
- [issue-targetVersionElement](#issue-targetversionelement) — 5 properties
- [issueCollection](#issuecollection) — 6 properties
- [issueSelectOptions](#issueselectoptions) — 24 properties

## issue

Browser definition `issue`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assigned` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `bFixed` | Fixed | boolean |  |  |  |  |
| `brokenInVersion` |  | issue-brokenInVersionCollection |  |  | [`issue-brokenInVersionCollection`](#issue-brokeninversioncollection) |  |
| `brokenMandatory` | Broken In Mandatory | string |  |  |  |  |
| `buildBroken` | Broken In Build | string |  |  |  |  |
| `buildFixed` | Fixed In Build | string |  |  |  |  |
| `buildTarget` | Target Build | string |  |  |  |  |
| `closedDate` | Closed Date | string | date-time |  |  |  |
| `createdDate` | Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateReleased` | Date Released | string |  |  |  |  |
| `duplicateStatus` | Duplicate | string |  |  |  |  |
| `emailAssignee` | Email Assignee | boolean |  |  |  |  |
| `externalAbstract` | External Abstract | string |  |  |  |  |
| `externalDetails` | External Details | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fixedInVersion` |  | issue-fixedInVersionCollection |  |  | [`issue-fixedInVersionCollection`](#issue-fixedinversioncollection) |  |
| `fixedMandatory` | Fixed In Mandatory | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isOwner` | I Own This Issue | boolean |  |  |  |  |
| `isReviewed` | Reviewed | boolean |  |  |  |  |
| `isShowstopper` | Showstopper | boolean |  |  |  |  |
| `issueAbstract` | Abstract | string |  |  |  |  |
| `issueCases` |  | supportCaseCollection |  |  | [`supportCaseCollection`](supportCase.md#supportcasecollection) |  |
| `issueNumber` | ID | string |  |  |  |  |
| `issueStatus` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `issueTags` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `issueType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `issueVersion` | Issue version | integer | int64 |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Modification Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mediaItem` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `module` | Module | string |  |  |  |  |
| `newDetails` | New Details | string |  |  |  |  |
| `origissueNumber` | Issue Number (Original) | string |  |  |  |  |
| `priority` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `product` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `productTeam` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedIssues` |  | issue-relatedIssuesCollection |  |  | [`issue-relatedIssuesCollection`](#issue-relatedissuescollection) |  |
| `reportedBy` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `reproduce` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `reviewer` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `severity` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `source` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `statusType` | Status Type | string |  |  |  |  |
| `targetMandatory` | Target Mandatory | string |  |  |  |  |
| `targetVersion` |  | issue-targetVersionCollection |  |  | [`issue-targetVersionCollection`](#issue-targetversioncollection) |  |
| `trackCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `tracking` | Tracking | boolean |  |  |  |  |
| `versionBroken` | Broken In Version | string |  |  |  |  |
| `versionFixed` | Fixed In Version | string |  |  |  |  |
| `versionTarget` | Target Version | string |  |  |  |  |

## issue-brokenInVersionCollection

Browser definition `issue-brokenInVersionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | issue-brokenInVersionElement[] |  |  | [`issue-brokenInVersionElement`](#issue-brokeninversionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## issue-brokenInVersionElement

Browser definition `issue-brokenInVersionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `build` | Build | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `primary` | Primary | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `version` | Version | string |  |  |  |  |

## issue-fixedInVersionCollection

Browser definition `issue-fixedInVersionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | issue-fixedInVersionElement[] |  |  | [`issue-fixedInVersionElement`](#issue-fixedinversionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## issue-fixedInVersionElement

Browser definition `issue-fixedInVersionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `build` | Build | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `primary` | Primary | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `version` | Version | string |  |  |  |  |

## issue-relatedIssuesCollection

Browser definition `issue-relatedIssuesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | issue-relatedIssuesElement[] |  |  | [`issue-relatedIssuesElement`](#issue-relatedissueselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## issue-relatedIssuesElement

Browser definition `issue-relatedIssuesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `duplicatedBy` | Duplicate | string |  |  |  |  |
| `issueAbstract` | Abstract | string |  |  |  |  |
| `issueAssignee` | Assigned To | string |  |  |  |  |
| `issueNumber` | Issue No. | string |  |  |  |  |
| `issueStatus` | Status | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relationship` |  | object |  |  |  |  |
| `relationship.id` | Internal identifier | string |  |  |  | `S3`, `S4`, `S5`, `S6`, `M1`, `M2`, `M3`, `M4`, `M5`, `M6`, `S2` |
| `relationship.refName` | Reference Name | string |  |  |  |  |
| `relationshipComment` | Comment | string |  |  |  |  |

## issue-targetVersionCollection

Browser definition `issue-targetVersionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | issue-targetVersionElement[] |  |  | [`issue-targetVersionElement`](#issue-targetversionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## issue-targetVersionElement

Browser definition `issue-targetVersionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `build` | Build | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `primary` | Primary | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `version` | Version | string |  |  |  |  |

## issueCollection

Browser definition `issueCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | issue[] |  |  | [`issue`](#issue) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## issueSelectOptions

Browser definition `issueSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assigned` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buildBroken` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buildFixed` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buildTarget` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueCases` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueTags` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `mediaItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `module` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `product` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `productTeam` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reportedBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reproduce` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `reviewer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `severity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `trackCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `versionBroken` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `versionFixed` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `versionTarget` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
