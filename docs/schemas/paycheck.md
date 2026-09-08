# Schemas: paycheck

Property tables for definitions owned by `paycheck`.

Record page: [paycheck](../records/paycheck.md).

## Index

- [paycheck](#paycheck) — 41 properties
- [paycheck-payContribCollection](#paycheck-paycontribcollection) — 6 properties
- [paycheck-payContribElement](#paycheck-paycontribelement) — 11 properties
- [paycheck-payDeductCollection](#paycheck-paydeductcollection) — 6 properties
- [paycheck-payDeductElement](#paycheck-paydeductelement) — 11 properties
- [paycheck-payDisburseCollection](#paycheck-paydisbursecollection) — 6 properties
- [paycheck-payDisburseElement](#paycheck-paydisburseelement) — 7 properties
- [paycheck-payEarnCollection](#paycheck-payearncollection) — 6 properties
- [paycheck-payEarnElement](#paycheck-payearnelement) — 16 properties
- [paycheck-payExpCollection](#paycheck-payexpcollection) — 6 properties
- [paycheck-payExpElement](#paycheck-payexpelement) — 9 properties
- [paycheck-payPtoCollection](#paycheck-payptocollection) — 6 properties
- [paycheck-payPtoElement](#paycheck-payptoelement) — 7 properties
- [paycheck-paySummaryCollection](#paycheck-paysummarycollection) — 6 properties
- [paycheck-paySummaryElement](#paycheck-paysummaryelement) — 11 properties
- [paycheck-payTaxCollection](#paycheck-paytaxcollection) — 6 properties
- [paycheck-payTaxElement](#paycheck-paytaxelement) — 17 properties
- [paycheck-payTimeCollection](#paycheck-paytimecollection) — 6 properties
- [paycheck-payTimeElement](#paycheck-paytimeelement) — 18 properties
- [paycheckCollection](#paycheckcollection) — 6 properties
- [paycheckSelectOptions](#paycheckselectoptions) — 11 properties

## paycheck

Browser definition `paycheck`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `address` | Address | string |  |  |  |  |
| `balance` | Balance | number | double |  |  |  |
| `batchNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `payContrib` |  | paycheck-payContribCollection |  |  | [`paycheck-payContribCollection`](#paycheck-paycontribcollection) |  |
| `payDeduct` |  | paycheck-payDeductCollection |  |  | [`paycheck-payDeductCollection`](#paycheck-paydeductcollection) |  |
| `payDisburse` |  | paycheck-payDisburseCollection |  |  | [`paycheck-payDisburseCollection`](#paycheck-paydisbursecollection) |  |
| `payEarn` |  | paycheck-payEarnCollection |  |  | [`paycheck-payEarnCollection`](#paycheck-payearncollection) |  |
| `payExp` |  | paycheck-payExpCollection |  |  | [`paycheck-payExpCollection`](#paycheck-payexpcollection) |  |
| `payFrequency` |  | object |  |  |  |  |
| `payFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `STARTOFPERIOD`, `WEEKLY`, `QUADWEEKLY`, `BIENNIALLY`, `DAILY`, `NEVER`, `ONETIME`, `SEMIANNUALLY`, `ENDOFPERIOD`, `MONTHLY`, `AUTOREFILL`, `TRIENNIALLY`, `HOURLY`, `QUARTERLY`, `ANNUALLY`, `CUSTOM`, `BIMONTHLY`, `BIWEEKLY` |
| `payFrequency.refName` | Reference Name | string |  |  |  |  |
| `payPto` |  | paycheck-payPtoCollection |  |  | [`paycheck-payPtoCollection`](#paycheck-payptocollection) |  |
| `paySummary` |  | paycheck-paySummaryCollection |  |  | [`paycheck-paySummaryCollection`](#paycheck-paysummarycollection) |  |
| `payTax` |  | paycheck-payTaxCollection |  |  | [`paycheck-payTaxCollection`](#paycheck-paytaxcollection) |  |
| `payTime` |  | paycheck-payTimeCollection |  |  | [`paycheck-payTimeCollection`](#paycheck-paytimecollection) |  |
| `periodEnding` | Period Ending | string | date |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` | Status | string |  |  |  |  |
| `statusRef` | Reference | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Check # | string |  |  |  |  |
| `userAmount` | Amount | number | double |  |  |  |
| `version` | Revision Count | integer | int64 |  |  |  |
| `workPlace` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## paycheck-payContribCollection

Browser definition `paycheck-payContribCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payContribElement[] |  |  | [`paycheck-payContribElement`](#paycheck-paycontribelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payContribElement

Browser definition `paycheck-payContribElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manualentry` | Manual Entry | boolean |  |  |  |  |
| `nid` | ID | integer | int64 |  |  |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `wagebase` | Wage Base | number | double |  |  |  |

## paycheck-payDeductCollection

Browser definition `paycheck-payDeductCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payDeductElement[] |  |  | [`paycheck-payDeductElement`](#paycheck-paydeductelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payDeductElement

Browser definition `paycheck-payDeductElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manualentry` | Manual Entry | boolean |  |  |  |  |
| `nid` | ID | integer | int64 |  |  |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `wagebase` | Wage Base | number | double |  |  |  |

## paycheck-payDisburseCollection

Browser definition `paycheck-payDisburseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payDisburseElement[] |  |  | [`paycheck-payDisburseElement`](#paycheck-paydisburseelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payDisburseElement

Browser definition `paycheck-payDisburseElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `bankAccountDecrypt` | Bank Account Number | string |  |  |  |  |
| `bankName` | Bank Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `method` | Payment Method | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `statusName` | Status | string |  |  |  |  |

## paycheck-payEarnCollection

Browser definition `paycheck-payEarnCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payEarnElement[] |  |  | [`paycheck-payEarnElement`](#paycheck-payearnelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payEarnElement

Browser definition `paycheck-payEarnElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `basedonquan` | Based on Quantity | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `count` | Hours/Base | number | float |  |  |  |
| `custjob` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `grossamount` | Amount | number | double |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manualentry` | Manual Entry | boolean |  |  |  |  |
| `nid` | ID | integer | int64 |  |  |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `payitemworkplace` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serviceItem` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |

## paycheck-payExpCollection

Browser definition `paycheck-payExpCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payExpElement[] |  |  | [`paycheck-payExpElement`](#paycheck-payexpelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payExpElement

Browser definition `paycheck-payExpElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `apply` | Pay | boolean |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nid` | ID | integer | int64 |  |  |  |
| `origdoc` | Orig Transaction Document | integer | int64 |  |  |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `transaction` | Transaction | string |  |  |  |  |

## paycheck-payPtoCollection

Browser definition `paycheck-payPtoCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payPtoElement[] |  |  | [`paycheck-payPtoElement`](#paycheck-payptoelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payPtoElement

Browser definition `paycheck-payPtoElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `hoursaccrued` | Hours Accrued | number | float |  |  |  |
| `hoursbalance` | Balance | number | float |  |  |  |
| `hoursused` | Hours Used | number | float |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nid` | ID | integer | int64 |  |  |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |

## paycheck-paySummaryCollection

Browser definition `paycheck-paySummaryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-paySummaryElement[] |  |  | [`paycheck-paySummaryElement`](#paycheck-paysummaryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-paySummaryElement

Browser definition `paycheck-paySummaryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `itemcategory` | Item Category | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `payitemtype` |  | object |  |  |  |  |
| `payitemtype.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `payitemtype.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sortcolumn` | Sort By | string |  |  |  |  |
| `value` | Value | number | double |  |  |  |
| `ytdAmount` | YTD Amount | number | double |  |  |  |

## paycheck-payTaxCollection

Browser definition `paycheck-payTaxCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payTaxElement[] |  |  | [`paycheck-payTaxElement`](#paycheck-paytaxelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payTaxElement

Browser definition `paycheck-payTaxElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `editable` | Edit | string |  |  |  |  |
| `isExempt` | Exempt | boolean |  |  |  |  |
| `isresidenttax` | Resident Status | boolean |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `nid` | ID | integer | int64 |  |  |  |
| `paytax` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reportablewagebase` | Reportable Wage Base | number | double |  |  |  |
| `sequence` | Sequence # | integer | int64 |  |  |  |
| `taxablewagebase` | Taxable Wage Base | number | double |  |  |  |
| `taxedwagebase` | Taxed Wage Base | number | double |  |  |  |

## paycheck-payTimeCollection

Browser definition `paycheck-payTimeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | paycheck-payTimeElement[] |  |  | [`paycheck-payTimeElement`](#paycheck-paytimeelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheck-payTimeElement

Browser definition `paycheck-payTimeElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `apply` | Pay | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `count` | Hours | number | float |  |  |  |
| `custjob` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `ddate` | Date | string | date |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `nid` | ID | integer | int64 |  |  |  |
| `origdoc` | Orig Transaction Document | integer | int64 |  |  |  |
| `origtimebreakdown` |  | integer | int64 |  |  |  |
| `payitem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `payitemworkplace` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serviceItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## paycheckCollection

Browser definition `paycheckCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | paycheck[] |  |  | [`paycheck`](#paycheck) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## paycheckSelectOptions

Browser definition `paycheckSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `batchNumber` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `payFrequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `workPlace` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
