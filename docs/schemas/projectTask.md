# Schemas: projectTask

Property tables for definitions owned by `projectTask`.

Record page: [projectTask](../records/projectTask.md).

## Index

- [projectTask](#projecttask) — 55 properties
- [projectTask-assigneeCollection](#projecttask-assigneecollection) — 6 properties
- [projectTask-assigneeElement](#projecttask-assigneeelement) — 17 properties
- [projectTask-predecessorCollection](#projecttask-predecessorcollection) — 6 properties
- [projectTask-predecessorElement](#projecttask-predecessorelement) — 9 properties
- [projectTaskCollection](#projecttaskcollection) — 6 properties
- [projectTaskSelectOptions](#projecttaskselectoptions) — 10 properties

## projectTask

Browser definition `projectTask`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `actualWork` | Actual Work | string |  |  |  |  |
| `allocatedWork` | Allocated Work | string |  |  |  |  |
| `assignee` |  | projectTask-assigneeCollection |  |  | [`projectTask-assigneeCollection`](#projecttask-assigneecollection) |  |
| `bBudgetUseCalculatedValues` | Use Calculated Values for all Labor Billing Budgets | boolean |  |  |  |  |
| `cBudgetUseCalculatedValues` | Use Calculated Values for all Labor Cost Budgets | boolean |  |  |  |  |
| `calculatedWork` | Calculated Work | number | float |  |  |  |
| `calculatedWorkBaseline` | Calculated Work Baseline | number | float |  |  |  |
| `constraintType` |  | object |  |  |  |  |
| `constraintType.id` | Internal identifier | string |  |  |  | `FIXEDSTART`, `ASAP` |
| `constraintType.refName` | Reference Name | string |  |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `duration` | Duration | string |  |  |  |  |
| `endDate` | End Date | string | date-time |  |  |  |
| `endDateBaseline` | End Date Baseline | string | date-time |  |  |  |
| `estimatedHoursAtCompletion` | Estimated Hours At Completion | string |  |  |  |  |
| `estimatedHoursToComplete` | Estimated Hours To Complete | string |  |  |  |  |
| `estimatedWork` | Estimated Work | number | float |  |  |  |
| `estimatedWorkBaseline` | Estimated Work Baseline | number | float |  |  |  |
| `eventId` | Project Task ID | integer | int64 |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `finishByDate` | Finish No Later Than | string | date |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `insertBefore` |  | projectTask |  |  | [`projectTask`](#projecttask) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Comments | string |  |  |  |  |
| `msprojoutlinenum` | MS Project Outline Number | string |  |  |  |  |
| `msprojpreds` | MS Project Predecessors | string |  |  |  |  |
| `msprojresources` | MS Project Resource Names | string |  |  |  |  |
| `msprojschedwork` | MS Project Scheduled Work | string |  |  |  |  |
| `msprojserviceitem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `msprojuid` | MS Project UID | string |  |  |  |  |
| `nonBillableTask` | Non-billable | boolean |  |  |  |  |
| `owner` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `parent` |  | projectTask |  |  | [`projectTask`](#projecttask) |  |
| `percentCompleteByRsrcAlloc` | Percent Complete by Allocated Work | number | double |  |  |  |
| `percentTimeComplete` | Percent Complete | number | double |  |  |  |
| `plannedWork` | Planned Work | string |  |  |  |  |
| `plannedWorkBaseline` | Planned Work Baseline | string |  |  |  |  |
| `plannedWorkTotal` | Planned Work Total | string |  |  |  |  |
| `predecessor` |  | projectTask-predecessorCollection |  |  | [`projectTask-predecessorCollection`](#projecttask-predecessorcollection) |  |
| `priority` |  | object |  |  |  |  |
| `priority.id` | Internal identifier | string |  |  |  | `HIGH`, `MEDIUM`, `LOW` |
| `priority.refName` | Reference Name | string |  |  |  |  |
| `project` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `remainingWork` | Remaining Work | string |  |  |  |  |
| `startDateBaseline` | Start Date Baseline | string | date-time |  |  |  |
| `startDateTime` | Start Date | string | date-time |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `NOTSTART`, `PROGRESS`, `COMPLETE` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `title` | Name | string |  |  |  |  |

## projectTask-assigneeCollection

Browser definition `projectTask-assigneeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | projectTask-assigneeElement[] |  |  | [`projectTask-assigneeElement`](#projecttask-assigneeelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## projectTask-assigneeElement

Browser definition `projectTask-assigneeElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billingClass` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `calculatedWork` | Calculated Work | number | float |  |  |  |
| `cost` | Cost | number | double |  |  |  |
| `createworkassignment` | Create Work Assignment | boolean |  |  |  |  |
| `estimatedWork` | Estimated Work | number | float |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `plannedWork` | Planned Work | number | float |  |  |  |
| `price` | Price | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `resource` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `resourceGroup` |  | resourceGroup |  |  | [`resourceGroup`](resourceGroup.md#resourcegroup) |  |
| `serviceItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `unitCost` | Unit Cost | number | double |  |  |  |
| `unitPrice` | Unit Price | number | double |  |  |  |
| `units` | Units | number | double |  |  |  |
| `workassignmentcount` | Work Assignments Count | integer | int64 |  |  |  |

## projectTask-predecessorCollection

Browser definition `projectTask-predecessorCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | projectTask-predecessorElement[] |  |  | [`projectTask-predecessorElement`](#projecttask-predecessorelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## projectTask-predecessorElement

Browser definition `projectTask-predecessorElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | End Date | string | date-time |  |  |  |
| `lagDays` | Lag Time | number | float |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `predecessor` |  | projectTask |  |  | [`projectTask`](#projecttask) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date-time |  |  |  |
| `type` |  | object |  |  |  |  |
| `type.id` | Internal identifier | string |  |  |  | `FS`, `SS`, `FF`, `SF` |
| `type.refName` | Reference Name | string |  |  |  |  |

## projectTaskCollection

Browser definition `projectTaskCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | projectTask[] |  |  | [`projectTask`](#projecttask) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## projectTaskSelectOptions

Browser definition `projectTaskSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `constraintType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertBefore` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `msprojserviceitem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `owner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `project` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
