# Schemas: employee

Property tables for definitions owned by `employee`.

Record page: [employee](../records/employee.md).

## Index

- [employee](#employee) — 186 properties
- [employee-accruedTimeCollection](#employee-accruedtimecollection) — 6 properties
- [employee-accruedTimeElement](#employee-accruedtimeelement) — 19 properties
- [employee-addressBook-addressBookAddress](#employee-addressbook-addressbookaddress) — 18 properties
- [employee-addressBookCollection](#employee-addressbookcollection) — 6 properties
- [employee-addressBookElement](#employee-addressbookelement) — 11 properties
- [employee-campaignsCollection](#employee-campaignscollection) — 6 properties
- [employee-campaignsElement](#employee-campaignselement) — 2 properties
- [employee-companyContributionCollection](#employee-companycontributioncollection) — 6 properties
- [employee-companyContributionElement](#employee-companycontributionelement) — 13 properties
- [employee-corporatecardsCollection](#employee-corporatecardscollection) — 6 properties
- [employee-corporatecardsElement](#employee-corporatecardselement) — 5 properties
- [employee-currencylistCollection](#employee-currencylistcollection) — 6 properties
- [employee-currencylistElement](#employee-currencylistelement) — 3 properties
- [employee-deductionCollection](#employee-deductioncollection) — 6 properties
- [employee-deductionElement](#employee-deductionelement) — 12 properties
- [employee-directDepositListCollection](#employee-directdepositlistcollection) — 6 properties
- [employee-directDepositListElement](#employee-directdepositlistelement) — 14 properties
- [employee-earningCollection](#employee-earningcollection) — 6 properties
- [employee-earningElement](#employee-earningelement) — 17 properties
- [employee-emergencycontactCollection](#employee-emergencycontactcollection) — 6 properties
- [employee-emergencycontactElement](#employee-emergencycontactelement) — 7 properties
- [employee-emppermsCollection](#employee-emppermscollection) — 6 properties
- [employee-emppermsElement](#employee-emppermselement) — 9 properties
- [employee-formw2Collection](#employee-formw2collection) — 6 properties
- [employee-formw2Element](#employee-formw2element) — 5 properties
- [employee-hcmpositionCollection](#employee-hcmpositioncollection) — 6 properties
- [employee-hcmpositionElement](#employee-hcmpositionelement) — 13 properties
- [employee-hreducationCollection](#employee-hreducationcollection) — 6 properties
- [employee-hreducationElement](#employee-hreducationelement) — 6 properties
- [employee-ratesCollection](#employee-ratescollection) — 6 properties
- [employee-ratesElement](#employee-rateselement) — 4 properties
- [employee-rolesCollection](#employee-rolescollection) — 6 properties
- [employee-rolesElement](#employee-roleselement) — 9 properties
- [employee-subscriptionMessageHistoryCollection](#employee-subscriptionmessagehistorycollection) — 6 properties
- [employee-subscriptionMessageHistoryElement](#employee-subscriptionmessagehistoryelement) — 2 properties
- [employee-subscriptionsCollection](#employee-subscriptionscollection) — 6 properties
- [employee-subscriptionsElement](#employee-subscriptionselement) — 5 properties
- [employeeCollection](#employeecollection) — 6 properties
- [employeeSelectOptions](#employeeselectoptions) — 47 properties

## employee

Browser definition `employee`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountNumber` | Account | string |  |  |  |  |
| `accruedTime` |  | employee-accruedTimeCollection |  |  | [`employee-accruedTimeCollection`](#employee-accruedtimecollection) |  |
| `addressBook` |  | employee-addressBookCollection |  |  | [`employee-addressBookCollection`](#employee-addressbookcollection) |  |
| `adpid` | ADP Id | string |  |  |  |  |
| `aliennumber` | Alien Number | string |  |  |  |  |
| `altName` | Employee | string |  |  |  |  |
| `approvallimit` | Expense Approval Limit | number | double |  |  |  |
| `approver` |  | employee |  |  | [`employee`](#employee) |  |
| `authworkdate` | Work Authorization Expiry Date | string | date |  |  |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `basewage` | Base Wage | number | float |  |  |  |
| `basewagetype` |  | object |  |  |  |  |
| `basewagetype.id` | Internal identifier | string |  |  |  | `annualsalary`, `hourly`, `monthlysalary` |
| `basewagetype.refName` | Reference Name | string |  |  |  |  |
| `billingClass` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `birthdate` | Birth Date | string | date |  |  |  |
| `bonustarget` | Bonus Target | number | float |  |  |  |
| `bonustargetcomment` | Target Comments | string |  |  |  |  |
| `bonustargetpayfrequency` |  | object |  |  |  |  |
| `bonustargetpayfrequency.id` | Internal identifier | string |  |  |  | `one_time`, `annually`, `monthly`, `quarterly` |
| `bonustargetpayfrequency.refName` | Reference Name | string |  |  |  |  |
| `bonustargettype` |  | object |  |  |  |  |
| `bonustargettype.id` | Internal identifier | string |  |  |  | `percentage`, `amount` |
| `bonustargettype.refName` | Reference Name | string |  |  |  |  |
| `btemplate` | Employee is Template | string |  |  |  |  |
| `campaigns` |  | employee-campaignsCollection |  |  | [`employee-campaignsCollection`](#employee-campaignscollection) |  |
| `changedetails` | Change Reason Details | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `comments` | Notes | string |  |  |  |  |
| `commissionpaymentpreference` |  | object |  |  |  |  |
| `commissionpaymentpreference.id` | Internal identifier | string |  |  |  | `PAYROLL`, `AP` |
| `commissionpaymentpreference.refName` | Reference Name | string |  |  |  |  |
| `companyContribution` |  | employee-companyContributionCollection |  |  | [`employee-companyContributionCollection`](#employee-companycontributioncollection) |  |
| `concurrentwebservicesuser` | Concurrent Web Services User | boolean |  |  |  |  |
| `conflictresults` |  | string |  |  |  |  |
| `corporatecards` |  | employee-corporatecardsCollection |  |  | [`employee-corporatecardsCollection`](#employee-corporatecardscollection) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `currencylist` |  | employee-currencylistCollection |  |  | [`employee-currencylistCollection`](#employee-currencylistcollection) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `deduction` |  | employee-deductionCollection |  |  | [`employee-deductionCollection`](#employee-deductioncollection) |  |
| `defaultAddress` | Default Address | string |  |  |  |  |
| `defaultBillingAddress` | Default Billing Address | string |  |  |  |  |
| `defaultJobResourceRole` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultShippingAddress` | Default Shipping Address | string |  |  |  |  |
| `defaultacctcorpcardexp` |  | account |  |  | [`account`](account.md#account) |  |
| `defaultexpensereportcurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `directDeposit` | Use Direct Deposit | boolean |  |  |  |  |
| `directDepositList` |  | employee-directDepositListCollection |  |  | [`employee-directDepositListCollection`](#employee-directdepositlistcollection) |  |
| `driverslicensenumber` | Driver's License Number | string |  |  |  |  |
| `earning` |  | employee-earningCollection |  |  | [`employee-earningCollection`](#employee-earningcollection) |  |
| `effectivedatemode` |  | object |  |  |  |  |
| `effectivedatemode.id` | Internal identifier | string |  |  |  | `PAST`, `CURRENT`, `FUTURE` |
| `effectivedatemode.refName` | Reference Name | string |  |  |  |  |
| `eligibleforcommission` | Eligible for Commission | boolean |  |  |  |  |
| `email` | Email | string |  |  |  |  |
| `emergencycontact` |  | employee-emergencycontactCollection |  |  | [`employee-emergencycontactCollection`](#employee-emergencycontactcollection) |  |
| `empcenterqty` | Employee Center Current | string |  |  |  |  |
| `empcenterqtymax` | EMP_CENTER_MAX | string |  |  |  |  |
| `employeecertificate` | Reciprocal Agreement With {1} | boolean |  |  |  |  |
| `employeechangereason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `employeeftestatus` |  | object |  |  |  |  |
| `employeeftestatus.id` | Internal identifier | string |  |  |  | `NOT_APPLICABLE`, `NOT_ASSIGNED`, `UNDER_ALLOCATED`, `FULLY_ALLOCATED`, `OVER_ALLOCATED` |
| `employeeftestatus.refName` | Reference Name | string |  |  |  |  |
| `employeestatus` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `employeetype` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `empperms` |  | employee-emppermsCollection |  |  | [`employee-emppermsCollection`](#employee-emppermscollection) |  |
| `enabledeductionlimits` | Preference Field | boolean |  |  |  |  |
| `entityId` | Entity ID | string |  |  |  |  |
| `ethnicity` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `expenselimit` | Expense Limit | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `firstName` | First Name | string |  |  |  |  |
| `formw2` |  | employee-formw2Collection |  |  | [`employee-formw2Collection`](#employee-formw2collection) |  |
| `fulluserqty` | FullUser current | string |  |  |  |  |
| `fulluserqtymax` | FullUser max | string |  |  |  |  |
| `gender` |  | object |  |  |  |  |
| `gender.id` | Internal identifier | string |  |  |  | `b`, `ns`, `nb`, `m`, `f` |
| `gender.refName` | Reference Name | string |  |  |  |  |
| `giveAccess` | Login Access | boolean |  |  |  |  |
| `globalSubscriptionStatus` |  | object |  |  |  |  |
| `globalSubscriptionStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `globalSubscriptionStatus.refName` | Reference Name | string |  |  |  |  |
| `hcmposition` |  | employee-hcmpositionCollection |  |  | [`employee-hcmpositionCollection`](#employee-hcmpositioncollection) |  |
| `hireDate` | Hire Date | string | date |  |  |  |
| `homePhone` | Home Phone | string |  |  |  |  |
| `hreducation` |  | employee-hreducationCollection |  |  | [`employee-hreducationCollection`](#employee-hreducationcollection) |  |
| `i9verified` | I-9 Verified | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `image` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `inheritiprules` | Inherit Allowed IP Addresses from Company | boolean |  |  |  |  |
| `initials` | Initials | string |  |  |  |  |
| `ipaddressrule` | Extra Allowed IP Addresses | string |  |  |  |  |
| `isInactive` | Is Inactive | boolean |  |  |  |  |
| `isJobManager` | Job Manager | boolean |  |  |  |  |
| `isJobResource` | Job Resource | boolean |  |  |  |  |
| `isempcenterqtyenforced` | Employee Center Enforce | string |  |  |  |  |
| `isfulluserqtyenforced` | FullUser enforce | string |  |  |  |  |
| `isretailuserqtyenforced` | RetailUser enforce | string |  |  |  |  |
| `issalesrep` | Sales Rep | boolean |  |  |  |  |
| `issupportrep` | Support Rep | boolean |  |  |  |  |
| `job` |  | hcmJob |  |  | [`hcmJob`](hcmJob.md#hcmjob) |  |
| `jobdescription` | Job Description | string |  |  |  |  |
| `jobemploymentcategory` |  | object |  |  |  |  |
| `jobemploymentcategory.id` | Internal identifier | string |  |  |  | `-10`, `-11` |
| `jobemploymentcategory.refName` | Reference Name | string |  |  |  |  |
| `jobid` | Job ID | string |  |  |  |  |
| `laborCost` | Labor Cost | number | double |  |  |  |
| `laborcategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `lastName` | Last Name | string |  |  |  |  |
| `lastPaidDate` | Last Paid Date | string | date |  |  |  |
| `lastReviewDate` | Last Review Date | string | date |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `maritalstatus` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `middleName` | Middle Name | string |  |  |  |  |
| `mobilePhone` | Mobile Phone | string |  |  |  |  |
| `nextReviewDate` | Next Review Date | string | date |  |  |  |
| `officePhone` | Office Phone | string |  |  |  |  |
| `overridecatchupamount` | Override Catch-Up Limit | number | double |  |  |  |
| `overridecatchupcheckbox` | Override Catch-Up Limit | boolean |  |  |  |  |
| `overrideelectivedeferralamount` | Override Elective Deferral Limit | number | double |  |  |  |
| `overrideelectivedeferralcheckbox` | Override Elective Deferral Limit | boolean |  |  |  |  |
| `overtimepolicy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `passportnumber` | Passport Number | string |  |  |  |  |
| `password` | Password | string |  |  |  |  |
| `password2` | Confirm Password | string |  |  |  |  |
| `payFrequency` |  | object |  |  |  |  |
| `payFrequency.id` | Internal identifier | string |  |  |  | `SEMIMONTHLY`, `WEEKLY`, `ANNUALLY`, `QUARTERLY`, `QUADWEEKLY`, `DAILY`, `NEVER`, `SEMIANNUALLY`, `MONTHLY`, `BIMONTHLY`, `BIWEEKLY` |
| `payFrequency.refName` | Reference Name | string |  |  |  |  |
| `phone` | Phone | string |  |  |  |  |
| `phoneticName` | Furigana | string |  |  |  |  |
| `purchaseorderapprovallimit` | Purchase Approval Limit | number | double |  |  |  |
| `purchaseorderapprover` |  | employee |  |  | [`employee`](#employee) |  |
| `purchaseorderlimit` | Purchase Limit | number | double |  |  |  |
| `rate` | Hourly Rate | number | double |  |  |  |
| `rates` |  | employee-ratesCollection |  |  | [`employee-ratesCollection`](#employee-ratescollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `releasedate` | Termination/Release Date | string | date |  |  |  |
| `requirePwdChange` | Require Password Change On Next Login | boolean |  |  |  |  |
| `residentstatus` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `retailuserqty` | RetailUser current | string |  |  |  |  |
| `retailuserqtymax` | RetailUser max | string |  |  |  |  |
| `roles` |  | employee-rolesCollection |  |  | [`employee-rolesCollection`](#employee-rolescollection) |  |
| `salesrole` |  | salesRole |  |  | [`salesRole`](salesRole.md#salesrole) |  |
| `salutation` | Mr./Ms... | string |  |  |  |  |
| `sendEmail` | Send New Access Notification Email | boolean |  |  |  |  |
| `socialsecuritynumber` | Social Security Number | string |  |  |  |  |
| `startdatetimeoffcalc` | Start Date for Time-Off Calculations | string | date |  |  |  |
| `subscriptionMessageHistory` |  | employee-subscriptionMessageHistoryCollection |  |  | [`employee-subscriptionMessageHistoryCollection`](#employee-subscriptionmessagehistorycollection) |  |
| `subscriptions` |  | employee-subscriptionsCollection |  |  | [`employee-subscriptionsCollection`](#employee-subscriptionscollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `supervisor` |  | employee |  |  | [`employee`](#employee) |  |
| `targetUtilization` | Target Utilization | number | double |  |  |  |
| `template` |  | employee |  |  | [`employee`](#employee) |  |
| `terminationbydeath` | Termination Due To Death | boolean |  |  |  |  |
| `terminationcategory` |  | object |  |  |  |  |
| `terminationcategory.id` | Internal identifier | string |  |  |  | `VOLUNTARY`, `INVOLUNTARY` |
| `terminationcategory.refName` | Reference Name | string |  |  |  |  |
| `terminationdetails` | Termination Details | string |  |  |  |  |
| `terminationreason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `terminationregretted` |  | object |  |  |  |  |
| `terminationregretted.id` | Internal identifier | string |  |  |  | `NO`, `UNSPECIFIED`, `YES` |
| `terminationregretted.refName` | Reference Name | string |  |  |  |  |
| `timeapprover` |  | employee |  |  | [`employee`](#employee) |  |
| `timeoffplan` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `title` | Job Title | string |  |  |  |  |
| `unsubscribe` | Unsubscribe from Campaigns | boolean |  |  |  |  |
| `usePerquest` | Include in Payroll | boolean |  |  |  |  |
| `useTimedata` |  | object |  |  |  |  |
| `useTimedata.id` | Internal identifier | string |  |  |  | `T`, `F` |
| `useTimedata.refName` | Reference Name | string |  |  |  |  |
| `visaexpdate` | Visa Expiration Date | string | date |  |  |  |
| `visatype` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `wasempcenterhasaccess` | Employee Center Has Access | string |  |  |  |  |
| `wasfulluserhasaccess` | FullUser hasaccess | string |  |  |  |  |
| `wasinactive` | wasinactive | string |  |  |  |  |
| `wasretailuserhasaccess` | RetailUser hasaccess | string |  |  |  |  |
| `workCalendar` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `workassignment` |  | object |  |  |  |  |
| `workassignment.id` | Internal identifier | string |  |  |  | `job`, `position` |
| `workassignment.refName` | Reference Name | string |  |  |  |  |
| `workplace` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## employee-accruedTimeCollection

Browser definition `employee-accruedTimeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-accruedTimeElement[] |  |  | [`employee-accruedTimeElement`](#employee-accruedtimeelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-accruedTimeElement

Browser definition `employee-accruedTimeElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accrualMethod` |  | object |  |  |  |  |
| `accrualMethod.id` | Internal identifier | string |  |  |  | `StartYear`, `EveryPeriod`, `Hourly` |
| `accrualMethod.refName` | Reference Name | string |  |  |  |  |
| `accrualRate` | Accrual Rate | number | float |  |  |  |
| `accruedHours` | Accrued Hours | number | float |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `maximumAccruedHours` | Maximum Hours | number | float |  |  |  |
| `monetaryRate` | Monetary Rate | number | double |  |  |  |
| `payType` |  | object |  |  |  |  |
| `payType.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `payType.refName` | Reference Name | string |  |  |  |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `peiKey` | ID | string |  |  |  |  |
| `piName` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `resetAccruedHoursAtYearEnd` | Reset at Year End | boolean |  |  |  |  |

## employee-addressBook-addressBookAddress

Browser definition `employee-addressBook-addressBookAddress`.

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

## employee-addressBookCollection

Browser definition `employee-addressBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-addressBookElement[] |  |  | [`employee-addressBookElement`](#employee-addressbookelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-addressBookElement

Browser definition `employee-addressBookElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBookAddress` |  | employee-addressBook-addressBookAddress |  |  | [`employee-addressBook-addressBookAddress`](#employee-addressbook-addressbookaddress) |  |
| `addressBookAddress_text` | Address | string |  |  |  |  |
| `addressId` | Internal ID | string |  |  |  |  |
| `defaultBilling` | Home | boolean |  |  |  |  |
| `defaultShipping` | Default Shipping | boolean |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `label` | Label | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-campaignsCollection

Browser definition `employee-campaignsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-campaignsElement[] |  |  | [`employee-campaignsElement`](#employee-campaignselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-campaignsElement

Browser definition `employee-campaignsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-companyContributionCollection

Browser definition `employee-companyContributionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-companyContributionElement[] |  |  | [`employee-companyContributionElement`](#employee-companycontributionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-companyContributionElement

Browser definition `employee-companyContributionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `derivedratemultiplier` | Rate Multiplier | number | double |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `limit` | Limit | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `peiKey` | ID | string |  |  |  |  |
| `piName` | Name | string |  |  |  |  |
| `pinamelinked` | Derived From | string |  |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `w2name` | W-2 | string |  |  |  |  |

## employee-corporatecardsCollection

Browser definition `employee-corporatecardsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-corporatecardsElement[] |  |  | [`employee-corporatecardsElement`](#employee-corporatecardselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-corporatecardsElement

Browser definition `employee-corporatecardsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `corporatecardprofile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `embossedname` | Name on Card | string |  |  |  |  |
| `expiration` | Expiration Date | string | date |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-currencylistCollection

Browser definition `employee-currencylistCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-currencylistElement[] |  |  | [`employee-currencylistElement`](#employee-currencylistelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-currencylistElement

Browser definition `employee-currencylistElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-deductionCollection

Browser definition `employee-deductionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-deductionElement[] |  |  | [`employee-deductionElement`](#employee-deductionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-deductionElement

Browser definition `employee-deductionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `derivedratemultiplier` | Rate Multiplier | number | double |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `limit` | Limit | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `peiKey` | ID | string |  |  |  |  |
| `piName` | Name | string |  |  |  |  |
| `pinamelinked` | Derived From | string |  |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-directDepositListCollection

Browser definition `employee-directDepositListCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-directDepositListElement[] |  |  | [`employee-directDepositListElement`](#employee-directdepositlistelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-directDepositListElement

Browser definition `employee-directDepositListElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountprenoted` | Prenoted | boolean |  |  |  |  |
| `accountstatus` | Status | string |  |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `bankName` | Bank Name | string |  |  |  |  |
| `bankaccountnumber` | Account Number | string |  |  |  |  |
| `bankid` | Bank Number | string |  |  |  |  |
| `banknumber` | Transit Number | string |  |  |  |  |
| `bankroutingnumber` | Routing Number | string |  |  |  |  |
| `id` | ID | string |  |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `netaccount` | Net Account | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `savingsaccount` | Savings Account | boolean |  |  |  |  |

## employee-earningCollection

Browser definition `employee-earningCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-earningElement[] |  |  | [`employee-earningElement`](#employee-earningelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-earningElement

Browser definition `employee-earningElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `defaultEarning` | Default | boolean |  |  |  |  |
| `defaultHours` | Default Hours | number | float |  |  |  |
| `derivedratemultiplier` | Rate Multiplier | number | float |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `payrate` | Rate | number | float |  |  |  |
| `payrollItem` |  | payrollItem |  |  | [`payrollItem`](payrollItem.md#payrollitem) |  |
| `paytype` |  | object |  |  |  |  |
| `paytype.id` | Internal identifier | string |  |  |  | `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10` |
| `paytype.refName` | Reference Name | string |  |  |  |  |
| `peiKey` | ID | string |  |  |  |  |
| `piName` | Name | string |  |  |  |  |
| `pinamelinked` | Derived From | string |  |  |  |  |
| `primaryEarning` | Primary | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-emergencycontactCollection

Browser definition `employee-emergencycontactCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-emergencycontactElement[] |  |  | [`employee-emergencycontactElement`](#employee-emergencycontactelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-emergencycontactElement

Browser definition `employee-emergencycontactElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `address` | Emergency Address | string |  |  |  |  |
| `contact` | Name | string |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `phone` | Emergency Phone | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relationship` | Relationship | string |  |  |  |  |

## employee-emppermsCollection

Browser definition `employee-emppermsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-emppermsElement[] |  |  | [`employee-emppermsElement`](#employee-emppermselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-emppermsElement

Browser definition `employee-emppermsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `permKey1` |  | object |  |  |  |  |
| `permKey1.id` | Internal identifier | string |  |  |  | `LIST_UPSELLWIZARD`, `ADMI_PI_REMOVAL_RUN`, `REPO_BALANCESHEET`, `REPO_ISSUE`, `EDIT_FISCALCALENDAR`, `LIST_SALESCAMPAIGN`, `LIST_WORKPLACE`, `REPO_TAX`, `TRAN_ORDERRESERVATION`, `LIST_SCSNAPSHOT`, `LIST_RESOURCE`, `LIST_BASICGOVERNMENTISSUEDIDS`, `ADMI_EMPLOYEE_EXPENSE_SOURCE`, `REGT_ACCTREC`, `REGT_DEFEREXPENSE`, `LIST_FAXTEMPLATE`, `REPO_PROJECT_ACCOUNTING`, `ADMI_LOGIN_OAUTH2`, `REPO_AR`, `TRAN_FXREVAL`, `REPO_AP`, `ADMI_CUSTOMSCRIPT`, `ADMI_ENTITYACCOUNTMAPPING`, `ADMI_MHLEVEL`, `TRAN_GENERATECHARGES`, `TRAN_SALESORDCOMMITREVENUE`, `ADMI_MCP_SERVER`, `ADMI_TELEPHONY_SETUP`, `LIST_SHIPPARTSHIPMENT`, `ADMI_MANAGEROLES`, `REGT_LONGTERMLIAB`, `ADMI_CASETYPE`, `REGT_DEFERREVENUE`, `ADMI_SFASETUP`, `ADMI_ADVANCED_TEMPLATES`, `LIST_TAXENGINESELECTION`, `REPO_PAYROLL`, `TRAN_CHARGE`, `ADMI_SUITEANALYTICSCONNECT`, `TRAN_BINWKSHT`, `LIST_COMPANY_FEATURE_SETUP`, `REGT_EQUITY`, `TRAN_VPREPAPPRV`, `REGT_ACCTPAY`, `TRAN_INTERCOADJ`, `REGT_INCOME`, `LIST_TIMEOFFADMIN`, `ADMI_CUSTCOLUMNFIELD`, `REPO_PAYROLLW2`, `REPO_REVREC`, `LIST_ITEM_COLLECTION`, `LIST_ZONE`, `ADMI_TEXTENHANCE`, `ADMI_CSP_SETUP`, `ADMI_PROJECTTEMPLATE`, `TRAN_ORDRESVAPPRV`, `TRAN_SALESORDAPPRV`, `ADMI_RAG`, `ADMI_TIMEMODIFICATION`, `LIST_VENDOR_ACH`, `TRAN_TAXLIAB`, `ADMI_TWOFACTORAUTH`, `ADMI_IMPORTXML`, `LIST_ITEMPROCESSGROUP`, `REPO_WEBSITE`, `TRAN_PEJRNL`, `LIST_ALLGOVERNMENTISSUEDIDS`, `TRAN_COPY_BUDGET`, `LIST_SUPPLY_REALLOCATION`, `LIST_IMPORTED_EMPLOYEE_EXPENSE`, `ADMI_CUSTRECORDFORM`, `ADMI_OPENIDSSO`, `LIST_PDFTEMPLATE`, `TRAN_WORKORDISSUE`, `ADMI_CUSTOMER_SEGMENTS`, `LIST_PICKDECOMPOSITION`, `TRAN_OPPRTNTY`, `ADMI_STATETAXIMPORT`, `ADMI_ACCTSETUP`, `LIST_PLANNEDSTANDARDCOST`, `ADMI_ENABLEFEATURES`, `LIST_REVRECFIELDMAPPING`, `LIST_PDFMESSAGE`, `SYSTEM_STATUS`, `TRAN_PRINTCHECKSFORMS`, `ADMI_ALLOW_JS_HTML_UPLOAD`, `LIST_ENTITY_DUPLICATES`, `TRAN_BLANKORDAPPRV`, `TRAN_TIMEBILL`, `TRAN_ITEMRCPT`, `ADMI_CONVERTCLASSES`, `ADMI_CUSTCATEGORY`, `ADMI_SUBSIDIARYSETTINGSMANAGER`, `TRAN_OWNTRNSF`, `ADMI_CUSTEMAILLAYOUT`, `ADMI_ACCOUNTINGBOOK`, `TRAN_RECEIVEINBOUND`, `LIST_SUBSCRIPTIONCHANGEORDER`, `ADMI_CUSTOMERRULE`, `ADMI_CUSTFORM`, `TRAN_FFTREQ`, `ADMI_FFTEXCEPTIONREASON`, `TRAN_RECOG_GIFTCERT_INCOME`, `LIST_BOM`, `LIST_REVENUEELEMENT`, `TRAN_CHECK`, `LIST_SITEEMAILTEMPLATE`, `ADMI_VIEWACHACCOUNT`, `TRAN_WOCLOSE`, `ADMI_PENDINGBOOKJOURNAL`, `ADMI_BANK_CONNECTIVITY_CONFIG`, `LIST_INTERNALPUBLISH`, `TRAN_YTDADJST`, `ADMI_CONSOLIDATED`, `LIST_ITEM_REVISION`, `REPO_INTEGRATION`, `ADMI_ADVANCED_ORDER_MANAGEMENT`, `LIST_STOREITEMLISTLA`, `TRAN_VENDBILL`, `ADMI_TWOFACTORAUTHBASE`, `LIST_STORETAB`, `ADMI_CASEPRIORITY`, `ADMI_CAMPAIGNEMAIL`, `ADMI_WORKFLOW`, `LIST_SHORTCUT`, `TRAN_XMLDETAIL`, `TRAN_STATEMENT`, `LIST_CARDHOLDERAUTHENTICATION`, `LIST_HCMPOSITION`, `LIST_TABLEAU_WORKBOOK_EXPORT`, `LIST_PRICEBOOK`, `LIST_PROMOTIONCODE`, `LIST_CRMGROUP`, `ADMI_EMPLCATEGORY`, `LIST_EARLIEST_AVAILABILITY`, `ADMI_ITEMACCOUNTMAPPING`, `REPO_PANDL`, `TRAN_RTNAUTHCREDIT`, `LIST_PHASEDPROCESS`, `LIST_REVRECTREATMENT`, `LIST_MATERIALREQUIREMENTSPLAN`, `ADMI_TAXPERIODS`, `LIST_LICENSEPLATE`, `ADMI_PROVSN_TSTDRV`, `TRAN_TRANSFER`, `ADMI_SALESCHANNEL`, `ADMI_CENTERLINK`, `LIST_MESSAGE_UMD_UNRESTRICTED`, `LIST_ONBOARDING_TASK`, `ADMI_CUSTTRANFIELD`, `LIST_EMPLOYEECHANGEREASON`, `LIST_EMPLOYEE`, `TRAN_CUSTRFND`, `LIST_CONTACTROLE`, `REGT_OTHEXPENSE`, `REPO_CUSTOMIZATION`, `REPO_GL`, `LIST_CAMPAIGNHISTORY`, `LIST_ENTITYSUBSIDIARYRELATION`, `LIST_INVCOSTTEMPLATE`, `LIST_UPSELL`, `TRAN_BLANKORD`, `LIST_EMPLOYEESSN`, `TRAN_EDITBANKINGINFO`, `ADMI_CASERULE`, `LIST_SYSTEMEMAILTEMPLATE`, `LIST_NEWSITEM`, `LIST_QUANTITYPRICINGSCHEDULE`, `TRAN_SALESORDFULFILL`, `REGT_OTHINCOME`, `TRAN_WORKORDCOMPLETE`, `GRAP_INC`, `ADMI_CUSTLIST`, `LIST_CASE`, `ADMI_ENTITYSTATUS`, `TRAN_CASHRFND`, `LIST_MAILMERGE`, `TRAN_PURCHCON`, `LIST_COSTEDBOMINQUIRY`, `LIST_INFOITEMFORM`, `LIST_ITEM`, `LIST_RSSFEED`, `LIST_TAXSCHEDULE`, `LIST_RECOGNITIONEVENTTYPE`, `LIST_PAYMENT_CARD_TOKEN`, `ADMI_EMAILPWD`, `LIST_PRICEPLAN`, `ADMI_DEVICE_ID`, `LIST_TALENT_ADMINISTRATION`, `ADMI_CASESTATUS`, `ADMI_RECORDS_CATALOG`, `ADMI_REPOLAYOUTS`, `LIST_TEGATAACCOUNT`, `LIST_ISSUE`, `ADMI_ESCALATIONTERRITORY`, `ADMI_STORESEARCH`, `REPO_EMAIL`, `TRAN_POSTVENDORBILLVARIANCE`, `TRAN_TRNFRORD`, `ADMI_TSTDRV_MASTER`, `ADMI_STORESETUP`, `ADMI_SUITEAPP_MANAGEMENT`, `LIST_VENDOR`, `ADMI_APPDEFPKG`, `LIST_FILECABINET`, `ADMI_SUBLIST`, `TRAN_PURCHREQAPPRV`, `LIST_COMPETITOR`, `TRAN_INVADJST`, `TRAN_MGRFORECAST`, `TRAN_SALESORDINVOICE`, `LIST_TRANNUMBERAUDITLOG`, `ADMI_LOGIN_OAUTH`, `LIST_MESSAGE_UNRESTRICTED`, `LIST_ITEMTEMPLATE`, `TRAN_AUTO_CASH`, `ADMI_CREATEJOBSFROMSALESTRANS`, `LIST_CAMPAIGN`, `ADMI_NSASOIDCPROVIDER`, `REPO_PURCHASEORDER`, `ADMI_MANAGE_OAUTH2`, `LIST_CONTACT`, `LIST_MAILMESSAGE`, `ADMI_INTEGRAPP`, `LIST_PLANNEDREVENUE`, `TRAN_TIMEPOST`, `LIST_REVRECTREATMENTRULE`, `REGT_OTHCURRASSET`, `LIST_WBS`, `TRAN_PAYMENTRESULTPREVIEW`, `TRAN_PURCHORDRECEIVE`, `ADMI_CSVIMPORTPREF`, `TRAN_INVREVAL`, `LIST_PA_RECORDS`, `ADMI_BUNDLERAUDITTRAIL`, `LIST_FINHISTORY`, `TRAN_CUSTINVCAPPRV`, `ADMI_CUSTEVENTFIELD`, `LIST_MASSUPDATES`, `LIST_REVENUERECOGNITIONRULE`, `REPO_SNAPSHOTLEAD`, `ADMI_EMPLOYEECENTERPUBLISHING`, `ADMI_SWAPPRICES`, `ADMI_PERIODCLOSING`, `TRAN_FINCHRG`, `ADMI_PERIODOVERRIDE`, `ADMI_SUITECOMMERCEANALYTICS`, `TRAN_SALESORD`, `ADMI_ACCOUNTING`, `ADMI_CUSTRECORD`, `ADMI_ACCOUNTINGLIST`, `LIST_WORKCALENDAR`, `ADMI_FINCHARGEPREF`, `TRAN_PUJRNL`, `LIST_JOBREQUISITION`, `ADMI_CUSTOMSUBLIST`, `ADMI_MANAGEUSERS`, `TRAN_BALJRNAL`, `REGT_CREDCARD`, `LIST_COMPONENTWHEREUSEDINQUIRY`, `ADMI_MOBILE_ACCESS`, `LIST_WEBSITE`, `REPO_QUOTA`, `ADMI_VIEW_PAYMENT_CARD_TOKENS`, `ADMI_RESTWEBSERVICES`, `REPO_SNAPSHOTCASE`, `LIST_EMPLOYEECHANGEREQUEST`, `LIST_REALLOCATE_ORDER_ITEM`, `ADMI_CLASSESTOLOCS`, `LIST_BILLCAPTURE`, `TRAN_WORKORDMARKBUILT`, `LIST_GLLINESAUDITLOGSEG`, `TRAN_ALLOCSCHEDULE`, `TRAN_TAXPYMT`, `ADMI_KEYS`, `LIST_INFOCATEGORY`, `ADMI_EMPLOYEELIST`, `REPO_CASHFLOW`, `LIST_PICKTASK`, `ADMI_PROJECT_ACCOUNTING_SETUP`, `LIST_COLORTHEME`, `REPO_WEBSTORE`, `ADMI_TRAN_ACCOUNTING_RULES`, `TRAN_CARDRFND`, `TRAN_EXPREPT`, `ADMI_GAINLOSSACCTMAPPING`, `LIST_TIMEOFF`, `REPO_PAYROLLHIDEFINEMPINFO`, `LIST_COMPANY`, `LIST_CALENDAR`, `ADMI_CUSTFIELD`, `TRAN_LIABPYMT`, `REPO_WORKFORCEANALYTICS`, `ADMI_NEXT_LANDINGPAGE`, `ADMI_ORDERALLOCATIONSTRATEGY`, `ADMI_TEAMSELLINGCONTRIBUTION`, `TRAN_VENDAUTHAPPRV`, `LIST_REVENUEPLAN`, `LIST_GIFT_CERTIFICATE`, `REGT_UNBILLEDREC`, `LIST_PRICINGRECORDS`, `ADMI_CERTIFICATES`, `ADMI_MANAGE_OAUTH_TOKENS`, `LIST_SUBSIDIARY`, `LIST_CRMTEMPLATE`, `ADMI_AUDITLOGIN`, `ADMI_ISSUEOBFUSCATEMASSUPDATE`, `REPO_SCHEDULE`, `ADMI_OPENIDSSOSETUP`, `ADMI_BALANCE_TRX_BY_SEGMENTS`, `LIST_EMPLOYEE_SELF`, `ADMI_SUPPORTSETUP`, `TRAN_NETTSTLM`, `TRAN_WORKORD`, `TRAN_RTNAUTHRECEIVE`, `ADMI_CASETERRITORY`, `ADMI_IMPORTCSVFILE`, `ADMI_PARTNERCONTRIBUTION`, `REPO_AUTHPARTNERCOMMISSION`, `REPO_PAYROLLHOURSEARNING`, `ADMI_CLOSE`, `ADMI_CREATEPEER`, `LIST_TAXDETAILSTAB`, `LIST_SHIPITEM`, `ADMI_KERNEL`, `GRAP_NETWORTH`, `LIST_BIG_SEARCH`, `ADMI_CUSTADDRESSFORM`, `NONE_NEEDED`, `TRAN_REVARRNG`, `TRAN_REVCONTR`, `ADMI_GLOBALACCOUNTMAPPING`, `LIST_PROJECTTASK`, `TRAN_RTNAUTHAPPRV`, `ADMI_RECSYS`, `ADMI_CUSTBODYFIELD`, `TRAN_REVCOMRV`, `LIST_TEMPLATE_CATEGORY`, `LIST_REVRECVSOE`, `REPO_DEFERREDEXPENSE`, `LIST_KUDOS`, `LIST_BONUS`, `LIST_CONTACTSUBSIDIARYRELATION`, `LIST_PARTNERCOMMISSNRULES`, `LIST_SENTEMAIL`, `REPO_CONSOLIDATED_REPORTING`, `ADMI_PAYMENT_LINK_SETUP`, `TRAN_VENDAUTHRETURN`, `REPO_PURCHASES`, `ADMI_SS_NLCORP`, `LIST_CUSTPROFILE`, `ADMI_NUMBERING`, `LIST_DEPARTMENT`, `TRAN_CARDHOLDERAUTHENTICATION`, `REGT_PAYROLL`, `REGT_EXPENSE`, `REPO_INVENTORY`, `ADMI_SUBSIDIARYHIERARCHYMOD`, `TRAN_JOURNALAPPRV`, `ADMI_PROVSN_NEW_TSTDRV`, `TRAN_RTNAUTH`, `TRAN_INVCOUNT`, `REPO_UNBILLED`, `TRAN_XCHGREQUEST`, `LIST_CUSTRECORDENTRY`, `LIST_MEDIAITEMFOLDER`, `TRAN_PRICELIST`, `ADMI_CUSTLAYOUT`, `ADMI_WEBSERVICES`, `ADMI_CUSTOTHERFIELD`, `TRAN_BUILD`, `TRAN_VENDAUTH`, `TRAN_CUSTDEP`, `LIST_WORKASSIGNMENT`, `LIST_ACCOUNT`, `TRAN_WAVE`, `ADMI_OUTLOOKINTEGRATION`, `LIST_LOCATION`, `ADMI_ANALYTICS`, `ADMI_CREDITCARD`, `ADMI_IMPORTOVERRIDESSTRIG`, `LIST_KEYS`, `REPO_TRIALBALANCE`, `LIST_ALLOCSCHEDULE`, `ADMI_CUSTENTRYFORM`, `LIST_RELATEDITEMS`, `LIST_SUBSCRIPTIONPLAN`, `REPO_TRAN`, `ADMI_TYPE`, `LIST_ADDRESS`, `LIST_SUBSCRIPTION`, `REGT_OTHCURRLIAB`, `TRAN_EDITPROFILE`, `TRAN_WORKORDBUILD`, `LIST_EXPENSEPLAN`, `ADMI_DELETEDRECORD`, `TRAN_TIMER`, `LIST_ONBOARDING_ADMINISTRATION`, `TRAN_POSTPERIODS`, `TRAN_TRNFRORDAPPRV`, `GRAP_EXP`, `LIST_EXPENSEAMORTIZATIONRULE`, `TRAN_ESTIMATE`, `ADMI_UNCATSITEITEMS`, `ADMI_CUSTITEMFIELD`, `LIST_CRMMESSAGE`, `TRAN_CARDHOLDERAUTHEVENT`, `REPO_PARTNERCOMMISSION`, `LIST_PROJECT_BUDGET`, `REPO_ANALYTICS`, `LIST_CONVERTLEAD`, `TRAN_VPREP`, `ADMI_VIEW_GENERAL_TOKENS`, `LIST_ITEMPROCESSFAMILY`, `ADMI_REMINDERS`, `ADMI_SETUPCOMPANY`, `ADMI_CASEORIGIN`, `ADMI_CONVERTLEAD`, `LIST_INFOITEM`, `LIST_EMPLOYEE_ADMINISTRATION`, `TRAN_NETTINGSETTLEMENTAPPRV`, `ADMI_ACCTPERIODS`, `ADMI_SS_SCHEDULING`, `ADMI_WEBSERVICESOVERRIDESSTRIG`, `LIST_DISTRIBUTIONNETWORK`, `LIST_SALESROLE`, `TRAN_VENDPYMT`, `LIST_TAXITEM`, `REPO_SALESORDER`, `TRAN_PARTNERCOMMISSN`, `LIST_FISCALCALENDAR`, `TRAN_PURCHORD`, `ADMI_CAMPAIGNSETUP`, `ADMI_FINANCIALINSTITUTION`, `TRAN_WOCOMPL`, `TRAN_CUSTPYMT`, `ADMI_PI_REMOVAL_CREATE`, `LIST_PI_ACCESS_LOG`, `LIST_PARTNER`, `REGT_FIXEDASSET`, `ADMI_CUSTFIELDTAB`, `LIST_FAIRVALUEPRICE`, `LIST_EMAILTEMPLATE`, `ADMI_PROVSN_QA`, `LIST_UNIT`, `TRAN_VENDCRED`, `REPO_RSRCALLOCATION`, `LIST_TASK`, `ADMI_BACKUPEXPORT`, `ADMI_BILLINGINFO`, `LIST_FIND`, `TRAN_STAXLIAB`, `ADMI_DUPLICATESETUP`, `TRAN_DEPOSIT`, `TRAN_INVWKSHT`, `LIST_RSRCALLOCATIONAPPRV`, `TRAN_VENDBILLAPPRV`, `REPO_RECONCILE`, `ADMI_MANAGE_OWN_OAUTH_TOKENS`, `TRAN_CLEARHOLD`, `ADMI_VIEW_VENDOR_ACH_ACCOUNT`, `LIST_EMPLOYEEEFFECTIVEDATING`, `ADMI_CROSSCHARGE`, `LIST_ONBOARDING_PLAN`, `LIST_OUTBOUNDREQUEST`, `ADMI_XMLADPSETUP`, `LIST_BILLINBOUNDSHIPMENT`, `ADMI_CUSTITEMNUMBERFIELD`, `TRAN_WORKORDMARKRELEASED`, `LIST_CASE_DUPLICATES`, `LIST_UNDELIVEREDEMAIL`, `REPO_AMORTIZATION`, `TRAN_MATCHING_RULES`, `REPO_NONPOSTING`, `ADMINDOCS`, `REPO_SUPPORT`, `ADMI_SAMLSSOSETUP`, `LIST_GENERICRESOURCE`, `ADMI_KPIREPORT`, `ADMI_SETUPIMAGERESIZE`, `TRAN_RFQ`, `ADMI_ADMINDOCSEU`, `LIST_STORECATEGORY`, `REPO_RETURNAUTH`, `ADMI_UNLOCKEDTIMEPERIOD`, `LIST_SAASMETRIC`, `ADMI_COPYPROJECTTASK`, `LIST_JOB`, `ADMI_SAVEDASHBOARD`, `LIST_GOVERNMENTISSUEDIDTYPE`, `LIST_EMPLOYEESEPARATION`, `ADMI_APPPUBLISHER`, `REGT_BANK`, `ADMI_OUTLOOKINTEGRATION_V3`, `LIST_GENERAL_TOKEN`, `TRAN_GATEWAYNOTIFICATION`, `REPO_W4`, `TRAN_WORKORDCLOSE`, `ADMI_MANAGE_OWN_OAUTH2_CERTS`, `LIST_CATEGORY`, `ADMI_SAC_READALL`, `LIST_OTHER_ADDRESS`, `LIST_PROJECTTEMPLATE`, `TRAN_UNBUILD`, `LIST_PAYMENT_INSTRUMENTS`, `ADMI_SNAPSHOTS`, `LIST_AUDITTRAIL`, `ADMI_SALESTERRITORY`, `LIST_INBOUNDSHIPMENT`, `LIST_MERGEPROLONGTIMEOUT`, `LIST_CLASS`, `REPO_TIME`, `LIST_SHIPPARTPACKAGE`, `ADMI_CASEFORM`, `TRAN_FORECAST`, `ADMI_UPDATEPRICES`, `TRAN_CUSTCHRG`, `TRAN_DEPAPPL`, `TRAN_APPROVECOMMISSN`, `LIST_NOTIFICATION`, `LIST_FAIRVALUEDIMENSION`, `REGT_OTHASSET`, `TRAN_CUSTCRED`, `TRAN_SYSJRNL`, `LIST_ANALYTICALIMPACT`, `TRAN_SALESORDREVENUECONTRACT`, `REPO_ACCOUNTDETAIL`, `ADMI_ADMINDOCSOTHER`, `ADMI_COMMISSIONSETUP`, `LIST_PROJECTREVENUERULE`, `TRAN_VENDAUTHCREDIT`, `TRAN_TEGRCVBL`, `ADMI_CUSTTASKS`, `LIST_RESOURCEGROUP`, `LIST_TALENT_EMPLOYEE`, `REPO_PAYROLLJOURNAL`, `TRAN_RTNAUTHREVERSEREVCOMMIT`, `ADMI_CUSTENTITYFIELD`, `TRAN_PAYMENTEVENT`, `ADMI_KNOWLEDGEBASE`, `TRAN_COMMISSN`, `LIST_CHECKITEMAVAILABILITY`, `LIST_SHIPPARTREGISTRATION`, `REPO_SALES_PARTNER`, `TRAN_REVARRNGAPPRV`, `TRAN_PURCHORDBILL`, `LIST_SYSTEMNOTES`, `LIST_INSTALLMENT_PAYMENT_LINKS`, `LIST_RSRCALLOCATION`, `LIST_ORGANIZATIONVALUE`, `ADMI_WEBSERVICESSETUP`, `LIST_RECORDCUSTFIELD`, `TRAN_VENDPYMTAPPRV`, `ADMI_MANAGEPERMISSIONS`, `ADMI_SITEMANAGEMENT`, `ADMI_CUSTCENTER`, `REGT_STAT`, `TRAN_ITEMSHIP`, `ADMI_CUSTPAGE`, `REGT_COGS`, `ADMI_UPSELLSETUP`, `LIST_HISTORY`, `LIST_MAILTEMPLATE`, `LIST_PAYMENT_CARD`, `TRAN_VPREPAPP`, `ADMI_BUNDLER`, `LIST_CUSTJOB`, `TRAN_TEGPYBL`, `REPO_PAYROLLLIAB`, `TRAN_REVCOMM`, `ADMI_CUSTSECTION`, `REPO_PAYCHECKDETAIL`, `TRAN_MANAGEPAYROLL`, `LIST_FORMW2`, `LIST_EMPLOYEECHANGETYPE`, `TRAN_PURCHCONAPPRV`, `ADMI_ISSUESETUP`, `ADMI_EXPENSEREPORTPOLICY`, `ADMI_MANUFACTURING`, `ADMI_MHNODE`, `LIST_EMPLOYEE_CONFIDENTIAL`, `LIST_FAXMESSAGE`, `TRAN_PAYROLLRUN`, `LIST_BILLOFMATERIALSINQUIRY`, `LIST_ITEMREVENUECATEGORY`, `TRAN_CARDCHRG`, `TRAN_PRINTSHIPMENTDOCS`, `TRAN_COMMITPAYROLL`, `TRAN_IMPORTOLBFILE`, `REPO_941`, `TRAN_WOISSUE`, `ADMI_IMPORTDEFAULT`, `REPO_940`, `TRAN_INVTRNFR`, `ADMI_SETUPYEARSTATUS`, `ADMI_DEPTSEGMENTMAPPING`, `ADMI_CLASSSEGMENTMAPPING`, `LIST_BIN`, `LIST_EMPLOYEE_PUBLIC`, `ADMI_PAYROLL`, `REPO_SALES_PROMO`, `TRAN_FIND`, `ADMI_COMMERCECATEGORY`, `TRAN_BALANCEOVERVIEW`, `TRAN_STATCHNG`, `REPO_SFA`, `REGT_NONPOSTING`, `TRAN_BINTRNFR`, `ADMI_VIEWCREDITCARDS`, `ADMI_ALLOWNONGLCHANGES`, `LIST_ORDER_REALLOCATION`, `REPO_TAXREPORTS`, `ADMI_LOCATIONCOSTINGGROUP`, `TRAN_STPICKUP`, `ADMI_APP_DEPLOYMENT`, `TRAN_GST_REFUND`, `ADMI_PROMPTS`, `TRAN_PROJECT_IC_CHARGE_REQUEST`, `LIST_PICKSTRATEGY`, `TRAN_CASHSALE`, `ADMI_SUITE_OAX_CONNECTOR`, `ADMI_DIRECTINVOICEPAYMENTSETUP`, `TRAN_OPENBAL`, `TRAN_QUOTA`, `LIST_GLOBALINVTRELATIONSHIP`, `LIST_PAYCHECK`, `LIST_OTHERNAME`, `REPO_MARKETING`, `LIST_BULK_PROCESSING`, `TRAN_CREATEINVCOUNT`, `LIST_OVERTIMEPOLICY`, `LIST_PAYMETH`, `ADMI_CUSTOMIZEDFIELDLEVELHELP`, `ADMI_SECRETS`, `LIST_MYROLES`, `ADMI_SAVE_HISTORICAL_METRICS`, `LIST_EXPORT`, `LIST_AMORTIZATION`, `ADMI_OIDCSETUP`, `ADMI_TAXMIGRATION`, `LIST_HCMJOB`, `REPO_PSTSUMMARY`, `ADMI_MANAGECUSTOMSEGMENTS`, `ADMI_COMPANY`, `ADMI_CUSTOMERFORM`, `ADMI_HTMLFORMULA`, `ADMI_USER`, `LIST_USAGE`, `TRAN_CUSTAUTH`, `REPO_REMINDEREMPLOYEE`, `ADMI_MIGRATEREVARRNGANDPLAN`, `REPO_PERIODENDFINANCIALS`, `LIST_EVENT`, `TRAN_INVDISTR`, `ADMI_OIDC`, `TRAN_PRINT`, `TRAN_CUSTINVC`, `ADMI_LOCSEGMENTMAPPING`, `REPO_BUDGET`, `TRAN_ORDRESV`, `ADMI_REVIEW_CUSTOM_GL_RUNS`, `LIST_BONUSTYPE`, `LIST_PUBLIC_TEMPLATE_CATEGORY`, `LIST_CALL`, `REPO_1099`, `ADMI_BLCGA`, `ADMI_CRMLIST`, `LIST_GLLINESAUDITLOG`, `TRAN_AUDIT`, `LIST_MFGCOSTTEMPLATE`, `TRAN_XCHGJRNL`, `ADMI_ADMINDOCSNA`, `LIST_CERTIFICATES`, `TRAN_PURCHREQ`, `LIST_BILLINGSCHEDULE`, `TRAN_CHARGERULE`, `LIST_BILLOFDISTRIBUTION`, `LIST_LABORCOSTING`, `LIST_COMMISSIONRULES`, `ADMI_VICARIOUS_EMAILS`, `REPO_COMMISSION`, `LIST_VENDOR_PAYMENT_INST`, `ADMI_DOMAINS`, `LIST_FINANCIAL_EXCEPTION_MGMT`, `LIST_ITEMDEMANDPLAN`, `LIST_CARDHOLDERAUTHEVENT`, `TRAN_AMENDW4`, `LIST_FAIRVALUEFORMULA`, `ADMI_WEBSERVICESLOG`, `TRAN_TIMECALC`, `TRAN_WORKORDMARKFIRMED`, `LIST_MEMDOC`, `LIST_ACH`, `LIST_ITEMSUPPLYPLAN`, `ADMI_ISSUESHOWSTOPPER`, `TRAN_PCHKJRNL`, `ADMI_TRANSITEMTXT`, `LIST_PUBLISHSEARCH`, `LIST_INTEGRAPP`, `LIST_STANDARDCOSTVERSION`, `REPO_FINANCIALS`, `ADMI_BUNDLERMANUP`, `TRAN_BUDGET`, `TRAN_PAYCHECK`, `GRAP_AP`, `LIST_CURRENCY`, `LIST_TIMECODE`, `GRAP_AR`, `LIST_ORDERMANAGEDASHBOARD`, `TRAN_APPROVEPARTNERCOMM`, `ADMI_ESCALATIONRULE`, `ADMI_SUPPLYALLOCATIONSETUP`, `ADMI_TRANSLATION`, `LIST_EMPLOYEE_RECORD`, `REPO_GSTSUMMARY`, `LIST_PAYROLLITEM`, `LIST_SCHEDULEMASSUPDATES`, `ADMI_REPOGROUPS`, `ADMI_CLOSEPERIOD`, `LIST_INVENTORYSTATUS`, `TRAN_ESTIMATEDCOSTOVERRIDE`, `ADMI_ORDERPROMISING`, `LIST_EMPLOYEE_ACCESS`, `TRAN_JOURNAL`, `TRAN_ADJUSTMENTJOURNAL`, `ADMI_USERPREF`, `ADMI_MHVERSION`, `TRAN_PAYMENTAUDIT`, `ADMI_STARTER_PROMPT_THEME`, `ADMI_SAMLSSO`, `LIST_PRESCATEGORY`, `TRAN_VENDRFQ`, `REPO_GRANT_ACCESS`, `ADMI_CUSTTRANSACTION`, `ADMI_CASEISSUE`, `ADMI_SUITESIGNON`, `REPO_PAYROLLSTATEWITHHOLD`, `REPO_BOOKINGS`, `LIST_KNOWLEDGEBASE`, `LIST_MFGROUTING`, `LIST_REVRECSCHEDULE`, `REPO_SALES`, `ADMI_PROVISION`, `ADMI_EXPORTIIF`, `ADMI_CASEALERT`, `TRAN_DLTD_TXNS_SUMMARY_SBMSN`, `TRAN_RECONCILE`, `ADMI_MANAGE_RESTRICTIONS` |
| `permKey1.refName` | Reference Name | string |  |  |  |  |
| `permLevel1` |  | object |  |  |  |  |
| `permLevel1.id` | Internal identifier | string |  |  |  | `0`, `1`, `2`, `3`, `4` |
| `permLevel1.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-formw2Collection

Browser definition `employee-formw2Collection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-formw2Element[] |  |  | [`employee-formw2Element`](#employee-formw2element) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-formw2Element

Browser definition `employee-formw2Element`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `download` | download | string |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `year` | Year | string |  |  |  |  |

## employee-hcmpositionCollection

Browser definition `employee-hcmpositionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-hcmpositionElement[] |  |  | [`employee-hcmpositionElement`](#employee-hcmpositionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-hcmpositionElement

Browser definition `employee-hcmpositionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `employmentCategory` |  | object |  |  |  |  |
| `employmentCategory.id` | Internal identifier | string |  |  |  | `-10`, `-11` |
| `employmentCategory.refName` | Reference Name | string |  |  |  |  |
| `fullTimeEquivalent` | Full Time Equivalent | number | float |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `position` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `positionAllocation` | Allocated Position FTE | number | float |  |  |  |
| `positionId` | Position ID | string |  |  |  |  |
| `primaryPosition` | Primary | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reportsTo` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## employee-hreducationCollection

Browser definition `employee-hreducationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-hreducationElement[] |  |  | [`employee-hreducationElement`](#employee-hreducationelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-hreducationElement

Browser definition `employee-hreducationElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `degree` | Degree | string |  |  |  |  |
| `degreeDate` | Date Conferred | string | date |  |  |  |
| `education` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nId` | Line Id | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-ratesCollection

Browser definition `employee-ratesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-ratesElement[] |  |  | [`employee-ratesElement`](#employee-rateselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-ratesElement

Browser definition `employee-ratesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `entityCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `rate` | Hourly Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-rolesCollection

Browser definition `employee-rolesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-rolesElement[] |  |  | [`employee-rolesElement`](#employee-roleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-rolesElement

Browser definition `employee-rolesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billingWarn` | <A href='/app/billing/billingterms.nl?user=T'>Charges may apply</a> | string |  |  |  |  |
| `centerType` |  | string |  |  |  |  |
| `deviceidOnly` |  | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `masterRole` |  | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `selectedRole` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `ssoOnly` |  | string |  |  |  |  |
| `wsOnly` |  | string |  |  |  |  |

## employee-subscriptionMessageHistoryCollection

Browser definition `employee-subscriptionMessageHistoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-subscriptionMessageHistoryElement[] |  |  | [`employee-subscriptionMessageHistoryElement`](#employee-subscriptionmessagehistoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-subscriptionMessageHistoryElement

Browser definition `employee-subscriptionMessageHistoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## employee-subscriptionsCollection

Browser definition `employee-subscriptionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | employee-subscriptionsElement[] |  |  | [`employee-subscriptionsElement`](#employee-subscriptionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employee-subscriptionsElement

Browser definition `employee-subscriptionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscribed` | Subscribed | boolean |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |

## employeeCollection

Browser definition `employeeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | employee[] |  |  | [`employee`](#employee) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## employeeSelectOptions

Browser definition `employeeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approver` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `basewagetype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingClass` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bonustargetpayfrequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bonustargettype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `commissionpaymentpreference` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultBillingAddress` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultJobResourceRole` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultShippingAddress` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultacctcorpcardexp` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultexpensereportcurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `effectivedatemode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employeechangereason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employeeftestatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employeestatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employeetype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ethnicity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `gender` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `globalSubscriptionStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `image` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `jobemploymentcategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `laborcategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `maritalstatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `overtimepolicy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `payFrequency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseorderapprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `residentstatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesrole` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supervisor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `template` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terminationcategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terminationreason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terminationregretted` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeapprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeoffplan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `useTimedata` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `visatype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `workCalendar` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `workassignment` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `workplace` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
