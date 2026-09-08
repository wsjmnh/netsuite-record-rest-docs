# Schemas: job

Property tables for definitions owned by `job`.

Record page: [job](../records/job.md).

## Index

- [job](#job) — 129 properties
- [job-addressBook-addressBookAddress](#job-addressbook-addressbookaddress) — 18 properties
- [job-addressBookCollection](#job-addressbookcollection) — 6 properties
- [job-addressBookElement](#job-addressbookelement) — 12 properties
- [job-bBudgetCollection](#job-bbudgetcollection) — 6 properties
- [job-bBudgetElement](#job-bbudgetelement) — 10 properties
- [job-cBudgetCollection](#job-cbudgetcollection) — 6 properties
- [job-cBudgetElement](#job-cbudgetelement) — 11 properties
- [job-paStatementCollection](#job-pastatementcollection) — 6 properties
- [job-paStatementElement](#job-pastatementelement) — 11 properties
- [job-percentCompleteOverrideCollection](#job-percentcompleteoverridecollection) — 6 properties
- [job-percentCompleteOverrideElement](#job-percentcompleteoverrideelement) — 8 properties
- [job-plStatementCollection](#job-plstatementcollection) — 6 properties
- [job-plStatementElement](#job-plstatementelement) — 12 properties
- [jobCollection](#jobcollection) — 6 properties
- [jobSelectOptions](#jobselectoptions) — 26 properties

## job

Browser definition `job`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountNumber` | Account | string |  |  |  |  |
| `actualTime` | Actual Work | string |  |  |  |  |
| `addressBook` |  | job-addressBookCollection |  |  | [`job-addressBookCollection`](#job-addressbookcollection) |  |
| `allocatedTime` | Allocated Work | string |  |  |  |  |
| `allowAllResourcesForTasks` | Display All Resources for Project Task Assignment | boolean |  |  |  |  |
| `allowExpenses` | Allow Expenses | boolean |  |  |  |  |
| `allowTaskTimeForRsrcAlloc` | Allow Allocated Resources to Enter Time to All Tasks | boolean |  |  |  |  |
| `allowTime` | Allow Time Entry | boolean |  |  |  |  |
| `altName` | Project | string |  |  |  |  |
| `applyProjectExpenseTypeToAll` | Apply to all time entries | boolean |  |  |  |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `averageProjectPlanRecalculationDuration` | Average Recalculation Duration | string |  |  |  |  |
| `bBudget` |  | job-bBudgetCollection |  |  | [`job-bBudgetCollection`](#job-bbudgetcollection) |  |
| `bBudgetUseCalculatedValues` | Use Calculated Values for all Billing Budgets | boolean |  |  |  |  |
| `baselineBudget` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `billingAccount` |  | billingAccount |  |  | [`billingAccount`](billingAccount.md#billingaccount) |  |
| `billingRateCard` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `cBudget` |  | job-cBudgetCollection |  |  | [`job-cBudgetCollection`](#job-cbudgetcollection) |  |
| `cBudgetLaborBudgetFromAlloc` | Calculate Labor Budgets from Resource Allocations | boolean |  |  |  |  |
| `cBudgetUseCalculatedValues` | Use Calculated Values for all Cost Budgets | boolean |  |  |  |  |
| `calculatedEndDate` | Calculated End Date | string | date |  |  |  |
| `calculatedEndDateBaseline` | Calculated End Date Baseline | string | date |  |  |  |
| `calculatedStartDate` | Calculated Start Date | string | date |  |  |  |
| `calculatedStartDateBaseline` | Calculated Start Date Baseline | string | date |  |  |  |
| `calculatedWork` | Calculated Work | string |  |  |  |  |
| `calculatedWorkBaseline` | Calculated Work Baseline | string |  |  |  |  |
| `category` |  | customerCategory |  |  | [`customerCategory`](customerCategory.md#customercategory) |  |
| `chargeAmountBilled` | Processed | number | double |  |  |  |
| `chargeAmountHoldForBilling` | Hold | number | double |  |  |  |
| `chargeAmountPending` | Total Pending Charges | number | double |  |  |  |
| `chargeAmountReadyForBilling` | Ready | number | double |  |  |  |
| `chargeAmountRemaining` | Remaining | number | double |  |  |  |
| `chargeExpenseAmount` | Expense | number | double |  |  |  |
| `chargeLaborAmount` | Labor | number | double |  |  |  |
| `comments` | Comments | string |  |  |  |  |
| `companyName` | Project Name | string |  |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contactList` |  | contactCollection |  |  | [`contactCollection`](contact.md#contactcollection) |  |
| `createChargeRule` | Create Charge Rule | boolean |  |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `defaultAddress` | Default Address | string |  |  |  |  |
| `defaultShippingAddress` | Default Shipping Address | string |  |  |  |  |
| `endDate` | Actual End Date | string | date |  |  |  |
| `entityId` | Entity ID | string |  |  |  |  |
| `entityStatus` |  | object |  |  |  |  |
| `entityStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5` |
| `entityStatus.refName` | Reference Name | string |  |  |  |  |
| `estimateAtCompletionBudget` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `estimateRevRecTemplate` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `estimatedCost` | Estimated Cost | number | double |  |  |  |
| `estimatedCostJc` | Estimated Cost | number | double |  |  |  |
| `estimatedGrossProfit` | Estimated Gross Profit | number | double |  |  |  |
| `estimatedGrossProfitPercent` | Estimated Gross Profit Percent | number | double |  |  |  |
| `estimatedLaborCost` | Estimated Labor Cost | number | double |  |  |  |
| `estimatedLaborCostBaseLine` | Estimated Labor Cost Baseline | number | double |  |  |  |
| `estimatedLaborRevenue` | Estimated Labor Revenue | number | double |  |  |  |
| `estimatedRevenue` | Estimated Revenue | number | double |  |  |  |
| `estimatedRevenueJc` | Estimated Revenue | number | double |  |  |  |
| `estimatedTime` | Initial Time Budget | string |  |  |  |  |
| `estimatedTimeOverride` | Estimated Work | string |  |  |  |  |
| `estimatedTimeOverrideBaseline` | Estimated Work Baseline | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `forecastChargeRunOnDemand` | Forecast Charge Run on Demand | boolean |  |  |  |  |
| `fxRate` | Exchange Rate | number | double |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeCrmTasksInTotals` | Include CRM Task In Project Totals | boolean |  |  |  |  |
| `isExemptTime` | Classify Time as Exempt | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isProductiveTime` | Classify Time as Productive | boolean |  |  |  |  |
| `isUtilizedTime` | Classify Time as Utilized | boolean |  |  |  |  |
| `jobBillingType` |  | object |  |  |  |  |
| `jobBillingType.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5` |
| `jobBillingType.refName` | Reference Name | string |  |  |  |  |
| `jobItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `jobPrice` | Project Price | number | double |  |  |  |
| `jobType` |  | jobType |  |  | [`jobType`](jobType.md#jobtype) |  |
| `language` |  | object |  |  |  |  |
| `language.id` | Internal identifier | string |  |  |  | `ro_RO`, `af_ZA`, `tl_PH`, `pt_BR`, `th_TH`, `bn_BD`, `cs_CZ`, `ca_ES`, `hu_HU`, `kn_IN`, `sk_SK`, `es_ES`, `nl_NL`, `te_IN`, `is_IS`, `sq_AL`, `sv_SE`, `es_AR`, `da_DK`, `ta_IN`, `sr_RS`, `en`, `ar`, `hr_HR`, `ko_KR`, `en_US`, `lt_LT`, `no_NO`, `it_IT`, `ru_RU`, `el_GR`, `pl_PL`, `en_AU`, `tr_TR`, `id_ID`, `hi_IN`, `mr_IN`, `ja_JP`, `fr_FR`, `he_IL`, `de_DE`, `ms_MY`, `zh_TW`, `fr_CA`, `pa_IN`, `fa_IR`, `bg_BG`, `vi_VN`, `hy_AM`, `lb_LU`, `sh_RS`, `ht_HT`, `fi_FI`, `en_GB`, `gu_IN`, `et_EE`, `en_CA`, `bs_BA`, `uk_UA`, `lv_LV`, `zh_CN`, `sl_SI`, `pt_PT` |
| `language.refName` | Reference Name | string |  |  |  |  |
| `lastBaseLineDate` | Last Baseline Date | string | date |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `lastProjectPlanRecalculationDateTime` | Last Recalculation | string | date-time |  |  |  |
| `lastProjectPlanRecalculationDuration` | Last Recalculation Duration | string |  |  |  |  |
| `lastProjectPlanRecalculationStatus` | Last Recalculation Status | string |  |  |  |  |
| `lastProjectPlanRecalculationTrigger` | Last Recalculation Trigger | string |  |  |  |  |
| `limitTimeToAssignees` | Limit Time and Expenses To Resources | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `materializeTime` | Create Planned Time Entries | boolean |  |  |  |  |
| `openingBalance` | Opening Balance | number | double |  |  |  |
| `openingBalanceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `openingBalanceDate` | Opening Balance Date | string | date |  |  |  |
| `paStatement` |  | job-paStatementCollection |  |  | [`job-paStatementCollection`](#job-pastatementcollection) |  |
| `parent` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `percentComplete` | Rev Rec Override Percent Complete | number | double |  |  |  |
| `percentCompleteByRsrcAlloc` | Percent Complete by Allocated Work | number | double |  |  |  |
| `percentCompleteOverride` |  | job-percentCompleteOverrideCollection |  |  | [`job-percentCompleteOverrideCollection`](#job-percentcompleteoverridecollection) |  |
| `percentTimeComplete` | Percent Work Complete | number | double |  |  |  |
| `plStatement` |  | job-plStatementCollection |  |  | [`job-plStatementCollection`](#job-plstatementcollection) |  |
| `plannedRevenue` | Planned Revenue | number | double |  |  |  |
| `plannedWork` | Planned Work | string |  |  |  |  |
| `plannedWorkBaseline` | Planned Work Baseline | string |  |  |  |  |
| `projectCompletelyBilled` | Project Completely Billed | boolean |  |  |  |  |
| `projectExpenseType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `projectManager` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `projectedEndDate` | Estimated End Date | string | date |  |  |  |
| `projectedEndDateBaseline` | Estimated End Date Baseline | string | date |  |  |  |
| `recognizedRevenue` | Recognize Revenue | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecForecastRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `scheduledEndDate` | Scheduled End Date | string | date |  |  |  |
| `scheduledEndDateBaseline` | Scheduled End Date Baseline | string | date |  |  |  |
| `schedulingMethod` |  | object |  |  |  |  |
| `schedulingMethod.id` | Internal identifier | string |  |  |  | `BACKWARD`, `FORWARD` |
| `schedulingMethod.refName` | Reference Name | string |  |  |  |  |
| `sourceServiceItemFromRateCard` | Source Service Item to Task Assignments from Rate Card | boolean |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `startDateBaseline` | Start Date Baseline | string | date |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `timeApproval` |  | object |  |  |  |  |
| `timeApproval.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `timeApproval.refName` | Reference Name | string |  |  |  |  |
| `timeRemaining` | Remaining Work | string |  |  |  |  |
| `totalRevenue` | Total (Revenue) | number | double |  |  |  |
| `useAllocatedTimeForForecast` | Use Allocated Time for Forecast | boolean |  |  |  |  |
| `usePercentCompleteOverride` | Use Percent Complete Override for Forecasting | boolean |  |  |  |  |
| `wbs` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## job-addressBook-addressBookAddress

Browser definition `job-addressBook-addressBookAddress`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addr1` | Address 1 | string |  |  |  |  |
| `addr2` | Address 2 | string |  |  |  |  |
| `addr3` | Address 3 | string |  |  |  |  |
| `addrPhone` | Phone | string |  |  |  |  |
| `addrText` | Address | string |  |  |  |  |
| `addressee` | Addressee | string |  |  |  |  |
| `attention` | Attention | string |  |  |  |  |
| `city` | City | string |  |  |  |  |
| `country` |  | object |  |  |  |  |
| `country.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `country.refName` | Reference Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `override` | Override | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `state` | State/Province | string |  |  |  |  |
| `zip` | Zip | string |  |  |  |  |

## job-addressBookCollection

Browser definition `job-addressBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | job-addressBookElement[] |  |  | [`job-addressBookElement`](#job-addressbookelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## job-addressBookElement

Browser definition `job-addressBookElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBookAddress` |  | job-addressBook-addressBookAddress |  |  | [`job-addressBook-addressBookAddress`](#job-addressbook-addressbookaddress) |  |
| `addressBookAddress_text` | Address | string |  |  |  |  |
| `addressId` | Internal ID | string |  |  |  |  |
| `defaultBilling` | Default Billing | boolean |  |  |  |  |
| `defaultShipping` | Default Shipping | boolean |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isResidential` | Residential Address | boolean |  |  |  |  |
| `label` | Label | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## job-bBudgetCollection

Browser definition `job-bBudgetCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | job-bBudgetElement[] |  |  | [`job-bBudgetElement`](#job-bbudgetelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## job-bBudgetElement

Browser definition `job-bBudgetElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `calculated` | Calculated | boolean |  |  |  |  |
| `categoryId` | Category ID | string |  |  |  |  |
| `categoryName` | Category | string |  |  |  |  |
| `costCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `month` | Month | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `yearMonth` | Month Date | string | date |  |  |  |

## job-cBudgetCollection

Browser definition `job-cBudgetCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | job-cBudgetElement[] |  |  | [`job-cBudgetElement`](#job-cbudgetelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## job-cBudgetElement

Browser definition `job-cBudgetElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `calculated` | Calculated | boolean |  |  |  |  |
| `calculatedFromAllocations` | Calculated from Allocations | boolean |  |  |  |  |
| `categoryId` | Category ID | string |  |  |  |  |
| `categoryName` | Category | string |  |  |  |  |
| `costCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `month` | Month | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `yearMonth` | Month Date | string | date |  |  |  |

## job-paStatementCollection

Browser definition `job-paStatementCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | job-paStatementElement[] |  |  | [`job-paStatementElement`](#job-pastatementelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## job-paStatementElement

Browser definition `job-paStatementElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `committedCost` | Committed Costs | number | double |  |  |  |
| `committedRevenue` | Committed Revenue | number | double |  |  |  |
| `cost` | Actual Cost | number | double |  |  |  |
| `isTotal` |  | string |  |  |  |  |
| `itemGroup` | Item Group | string |  |  |  |  |
| `job` |  | job |  |  | [`job`](#job) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `margin` | Margin | number | double |  |  |  |
| `profit` | Profit | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revenue` | Actual Revenue | number | double |  |  |  |

## job-percentCompleteOverrideCollection

Browser definition `job-percentCompleteOverrideCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | job-percentCompleteOverrideElement[] |  |  | [`job-percentCompleteOverrideElement`](#job-percentcompleteoverrideelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## job-percentCompleteOverrideElement

Browser definition `job-percentCompleteOverrideElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `calculatedPercentComplete` | Calculated percent complete | number | double |  |  |  |
| `comments` | Comments | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `percent` | Cumulative Percent Complete | number | double |  |  |  |
| `period` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `periodStatus` | Period Status | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revenuePlans` | Revenue Recognition Plans | number | double |  |  |  |

## job-plStatementCollection

Browser definition `job-plStatementCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | job-plStatementElement[] |  |  | [`job-plStatementElement`](#job-plstatementelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## job-plStatementElement

Browser definition `job-plStatementElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cost` | Cost | number | double |  |  |  |
| `costCategory` | Cost Category | string |  |  |  |  |
| `costCategoryRef` |  | integer | int64 |  |  |  |
| `costCategorySubtype` |  | string |  |  |  |  |
| `costCategoryType` |  | string |  |  |  |  |
| `isTotal` |  | string |  |  |  |  |
| `job` |  | job |  |  | [`job`](#job) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `margin` | Margin | number | double |  |  |  |
| `profit` | Profit | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revenue` | Revenue | number | double |  |  |  |

## jobCollection

Browser definition `jobCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | job[] |  |  | [`job`](#job) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## jobSelectOptions

Browser definition `jobSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `baselineBudget` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingRateCard` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultShippingAddress` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `estimateAtCompletionBudget` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `estimateRevRecTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `jobBillingType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `jobItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `jobType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `language` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `openingBalanceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `projectExpenseType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `projectManager` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecForecastRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `schedulingMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeApproval` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `wbs` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
