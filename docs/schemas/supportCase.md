# Schemas: supportCase

Property tables for definitions owned by `supportCase`.

Record page: [supportCase](../records/supportCase.md).

## Index

- [supportCase](#supportcase) — 72 properties
- [supportCase-escalateHistCollection](#supportcase-escalatehistcollection) — 6 properties
- [supportCase-escalateHistElement](#supportcase-escalatehistelement) — 8 properties
- [supportCase-statusHistoryCollection](#supportcase-statushistorycollection) — 6 properties
- [supportCase-statusHistoryElement](#supportcase-statushistoryelement) — 6 properties
- [supportCase-timeItemCollection](#supportcase-timeitemcollection) — 6 properties
- [supportCase-timeItemElement](#supportcase-timeitemelement) — 24 properties
- [supportCaseCollection](#supportcasecollection) — 6 properties
- [supportCaseSelectOptions](#supportcaseselectoptions) — 19 properties

## supportCase

Browser definition `supportCase`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assigned` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `caseNumber` | ID | string |  |  |  |  |
| `category` |  | supportCaseType |  |  | [`supportCaseType`](supportCaseType.md#supportcasetype) |  |
| `company` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `createdDate` | Creation Date/Time | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Creation Date/Time | string | date-time |  |  |  |
| `email` | Emails | string |  |  |  |  |
| `emailEmployees` | Copy Employees | string |  |  |  |  |
| `emailForm` | Email reply | boolean |  |  |  |  |
| `endDate` | Date Closed | string | date-time |  |  |  |
| `escalateHist` |  | supportCase-escalateHistCollection |  |  | [`supportCase-escalateHistCollection`](#supportcase-escalatehistcollection) |  |
| `escalateTo` |  | customerCollection |  |  | [`customerCollection`](customer.md#customercollection) |  |
| `escalationMessage` | Escalation Message | string |  |  |  |  |
| `eventNumber` | Number | integer | int64 |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `firstIssueAttached` | First Issue Attached | string | date-time |  |  |  |
| `firstIssueRemoved` | First Issue Removed | string | date-time |  |  |  |
| `firstUpdated` | First updated | string | date-time |  |  |  |
| `helpDesk` | Help Desk | boolean |  |  |  |  |
| `htmlMessage` | HTML Format | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inboundEmail` | Inbound Email Address | string |  |  |  |  |
| `incomingMessage` | Message | string |  |  |  |  |
| `initialResponseTime` | Initial Response Time | string |  |  |  |  |
| `internalOnly` | Internal Only | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `issue` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `issues` |  | issueCollection |  |  | [`issueCollection`](issue.md#issuecollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastCustomerMessageReceived` | Last Customer Message Received | string | date-time |  |  |  |
| `lastIssueAttached` | Last Issue Attached | string | date-time |  |  |  |
| `lastIssueRemoved` | Last Issue Removed | string | date-time |  |  |  |
| `lastMessageDate` | Last Message Date | string | date-time |  |  |  |
| `lastModifiedDate` | Last Modified Date/Time | string | date-time |  |  |  |
| `lastReopenedDate` | Date Last Reopened | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `mediaItem` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `messageNew` | New Message | boolean |  |  |  |  |
| `messageSave` | Messages | string |  |  |  |  |
| `module` | Module | string |  |  |  |  |
| `origCaseNumber` | Case Number (Original) | string |  |  |  |  |
| `origin` |  | supportCaseOrigin |  |  | [`supportCaseOrigin`](supportCaseOrigin.md#supportcaseorigin) |  |
| `outgoingMessage` | Reply | string |  |  |  |  |
| `phone` | Phone | string |  |  |  |  |
| `priority` |  | supportCasePriority |  |  | [`supportCasePriority`](supportCasePriority.md#supportcasepriority) |  |
| `product` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `profile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `quickNote` | Quick Note | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serialNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `solutions` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `spamLock` | Spam Lock | string |  |  |  |  |
| `stage` | Stage | string |  |  |  |  |
| `startDate` | Incident Date | string | date |  |  |  |
| `startTime` | Incident Time | string |  |  |  |  |
| `status` |  | supportCaseStatus |  |  | [`supportCaseStatus`](supportCaseStatus.md#supportcasestatus) |  |
| `statusHistory` |  | supportCase-statusHistoryCollection |  |  | [`supportCase-statusHistoryCollection`](#supportcase-statushistorycollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `supportFirstReply` | Support First Reply | string | date-time |  |  |  |
| `timeElapsed` | Time Elapsed | string |  |  |  |  |
| `timeItem` |  | supportCase-timeItemCollection |  |  | [`supportCase-timeItemCollection`](#supportcase-timeitemcollection) |  |
| `timeOnHold` | Time On Hold | string |  |  |  |  |
| `timeOpen` | Time Open | string |  |  |  |  |
| `timeToAssign` | Time To Assign | string |  |  |  |  |
| `timeToClose` | Time To Close | string |  |  |  |  |
| `title` | Subject | string |  |  |  |  |
| `transactionId` | Transaction ID | string |  |  |  |  |
| `useEmployeeTemplate` | Use Employee Template | boolean |  |  |  |  |
| `version` | Version | string |  |  |  |  |

## supportCase-escalateHistCollection

Browser definition `supportCase-escalateHistCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | supportCase-escalateHistElement[] |  |  | [`supportCase-escalateHistElement`](#supportcase-escalatehistelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCase-escalateHistElement

Browser definition `supportCase-escalateHistElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `action` | Action | string |  |  |  |  |
| `dateTime` | Date/Time | string | date-time |  |  |  |
| `fromEntity` | From | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Message | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `territory` | Escalation Assignment | string |  |  |  |  |
| `toEntity` | Escalate To | string |  |  |  |  |

## supportCase-statusHistoryCollection

Browser definition `supportCase-statusHistoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | supportCase-statusHistoryElement[] |  |  | [`supportCase-statusHistoryElement`](#supportcase-statushistoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCase-statusHistoryElement

Browser definition `supportCase-statusHistoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `date` | Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `stage` |  | object |  |  |  |  |
| `stage.id` | Internal identifier | string |  |  |  | `OPEN`, `CLOSED`, `ESCALATED` |
| `stage.refName` | Reference Name | string |  |  |  |  |

## supportCase-timeItemCollection

Browser definition `supportCase-timeItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | supportCase-timeItemElement[] |  |  | [`supportCase-timeItemElement`](#supportcase-timeitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCase-timeItemElement

Browser definition `supportCase-timeItemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `employee` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `externalId` | External ID | string |  |  |  |  |
| `hours` | Duration | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isExempt` | Exempt | boolean |  |  |  |  |
| `isProductive` | Productive | boolean |  |  |  |  |
| `isUtilized` | Utilized | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `overrideRate` | Lock this Rate | boolean |  |  |  |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `price` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `timeType` |  | object |  |  |  |  |
| `timeType.id` | Internal identifier | string |  |  |  | `P`, `A`, `B` |
| `timeType.refName` | Reference Name | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |

## supportCaseCollection

Browser definition `supportCaseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | supportCase[] |  |  | [`supportCase`](#supportcase) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## supportCaseSelectOptions

Browser definition `supportCaseSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assigned` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `company` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `escalateTo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issue` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issues` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `item` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `mediaItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `module` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `origin` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `product` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `profile` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `serialNumber` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `solutions` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
