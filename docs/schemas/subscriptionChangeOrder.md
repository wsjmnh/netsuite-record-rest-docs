# Schemas: subscriptionChangeOrder

Property tables for definitions owned by `subscriptionChangeOrder`.

Record page: [subscriptionChangeOrder](../records/subscriptionChangeOrder.md).

## Index

- [subscriptionChangeOrder](#subscriptionchangeorder) — 50 properties
- [subscriptionChangeOrder-changeOrderLineCollection](#subscriptionchangeorder-changeorderlinecollection) — 6 properties
- [subscriptionChangeOrder-changeOrderLineElement](#subscriptionchangeorder-changeorderlineelement) — 2 properties
- [subscriptionChangeOrder-newSubLineCollection](#subscriptionchangeorder-newsublinecollection) — 6 properties
- [subscriptionChangeOrder-newSubLineElement](#subscriptionchangeorder-newsublineelement) — 19 properties
- [subscriptionChangeOrder-renewalStepsCollection](#subscriptionchangeorder-renewalstepscollection) — 6 properties
- [subscriptionChangeOrder-renewalStepsElement](#subscriptionchangeorder-renewalstepselement) — 11 properties
- [subscriptionChangeOrder-subLineCollection](#subscriptionchangeorder-sublinecollection) — 6 properties
- [subscriptionChangeOrder-subLineElement](#subscriptionchangeorder-sublineelement) — 25 properties
- [subscriptionChangeOrderCollection](#subscriptionchangeordercollection) — 6 properties
- [subscriptionChangeOrderSelectOptions](#subscriptionchangeorderselectoptions) — 16 properties

## subscriptionChangeOrder

Browser definition `subscriptionChangeOrder`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `action` |  | object |  |  |  |  |
| `action.id` | Internal identifier | string |  |  |  | `ACTIVATE`, `MODIFY_PRICING`, `SUSPEND`, `REACTIVATE`, `RENEW`, `TERMINATE` |
| `action.refName` | Reference Name | string |  |  |  |  |
| `approvalDate` | Approval Date | string | date-time |  |  |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `PENDING_APPROVAL`, `APPROVED`, `REJECTED` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `billingAccount` |  | billingAccount |  |  | [`billingAccount`](billingAccount.md#billingaccount) |  |
| `changeOrderLine` |  | subscriptionChangeOrder-changeOrderLineCollection |  |  | [`subscriptionChangeOrder-changeOrderLineCollection`](#subscriptionchangeorder-changeorderlinecollection) |  |
| `createdBy` | Created By | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `idNumber` | Number | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `modificationType` |  | object |  |  |  |  |
| `modificationType.id` | Internal identifier | string |  |  |  | `NEW_CHURN`, `UPSELL_DOWNSELL`, `IGNORED` |
| `modificationType.refName` | Reference Name | string |  |  |  |  |
| `newSubLine` |  | subscriptionChangeOrder-newSubLineCollection |  |  | [`subscriptionChangeOrder-newSubLineCollection`](#subscriptionchangeorder-newsublinecollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `renewalEndDate` | Renewal End Date | string | date |  |  |  |
| `renewalMethod` |  | object |  |  |  |  |
| `renewalMethod.id` | Internal identifier | string |  |  |  | `EXTEND_EXISTING_SUBSCRIPTION`, `CREATE_NEW_SUBSCRIPTION` |
| `renewalMethod.refName` | Reference Name | string |  |  |  |  |
| `renewalPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |
| `renewalPriceBook` |  | priceBook |  |  | [`priceBook`](priceBook.md#pricebook) |  |
| `renewalStartDate` | Renewal Start Date | string | date |  |  |  |
| `renewalSteps` |  | subscriptionChangeOrder-renewalStepsCollection |  |  | [`subscriptionChangeOrder-renewalStepsCollection`](#subscriptionchangeorder-renewalstepscollection) |  |
| `renewalTerm` |  | subscriptionTerm |  |  | [`subscriptionTerm`](subscriptionTerm.md#subscriptionterm) |  |
| `renewalTranType` |  | object |  |  |  |  |
| `renewalTranType.id` | Internal identifier | string |  |  |  | `VendPymt`, `STaxLiab`, `CustCred`, `ItemShip`, `Check`, `RevContr`, `Journal`, `CustChrg`, `OrdResv`, `RevArrng`, `GLAdj`, `InvReval`, `Opprtnty`, `CustRfnd`, `CashRfnd`, `TrnfrOrd`, `Build`, `Unbuild`, `RevComm`, `SalesOrd`, `Rfq`, `VPrepApp`, `TegPybl`, `Deposit`, `WOIssue`, `FinChrg`, `PurchOrd`, `FftReq`, `StatChng`, `ExpRept`, `DepAppl`, `Wave`, `OwnTrnsf`, `StPickUp`, `TegRcvbl`, `WOCompl`, `NettStlm`, `InvAdjst`, `Transfer`, `Paycheck`, `BalJrnal`, `YtdAdjst`, `VendBill`, `XChgJrnl`, `ItemRcpt`, `Estimate`, `PChkJrnl`, `VPrep`, `SysJrnl`, `Commissn`, `TaxPymt`, `RtnAuth`, `CustInvc`, `FxReval`, `WorkOrd`, `PurchCon`, `BinTrnfr`, `LiaAdjst`, `InvDistr`, `VendRfq`, `LiabPymt`, `RevComRv`, `TaxLiab`, `InvcGrp`, `CuTrPrch`, `CustAuth`, `VendAuth`, `InvCount`, `InvWksht`, `CardRfnd`, `VendCred`, `PEJrnl`, `BinWksht`, `Custom`, `CustPymt`, `CustDep`, `PurchReq`, `WOClose`, `InbShip`, `CashSale`, `BlankOrd`, `CuTrSale`, `DeprCust`, `CardChrg`, `InvTrnfr` |
| `renewalTranType.refName` | Reference Name | string |  |  |  |  |
| `requestOffCycleInvoice` | Request Off-Cycle Invoice for Advance Charges | boolean |  |  |  |  |
| `requestor` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `saasCommitmentEffectiveDate` | SaaS Metric Commitment Effective Date | string | date |  |  |  |
| `saasCommitmentEndDate` | SaaS Metric Commitment End Date | string | date |  |  |  |
| `saasCommitmentStartDate` | SaaS Metric Commitment Start Date | string | date |  |  |  |
| `subLine` |  | subscriptionChangeOrder-subLineCollection |  |  | [`subscriptionChangeOrder-subLineCollection`](#subscriptionchangeorder-sublinecollection) |  |
| `subscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `subscriptionChangeOrderStatus` |  | object |  |  |  |  |
| `subscriptionChangeOrderStatus.id` | Internal identifier | string |  |  |  | `ACTIVE`, `VOIDED` |
| `subscriptionChangeOrderStatus.refName` | Reference Name | string |  |  |  |  |
| `subscriptionPlan` |  | subscriptionPlan |  |  | [`subscriptionPlan`](subscriptionPlan.md#subscriptionplan) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `terminateAtStartOfDay` | Effective at Start of day | boolean |  |  |  |  |

## subscriptionChangeOrder-changeOrderLineCollection

Browser definition `subscriptionChangeOrder-changeOrderLineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionChangeOrder-changeOrderLineElement[] |  |  | [`subscriptionChangeOrder-changeOrderLineElement`](#subscriptionchangeorder-changeorderlineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionChangeOrder-changeOrderLineElement

Browser definition `subscriptionChangeOrder-changeOrderLineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## subscriptionChangeOrder-newSubLineCollection

Browser definition `subscriptionChangeOrder-newSubLineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionChangeOrder-newSubLineElement[] |  |  | [`subscriptionChangeOrder-newSubLineElement`](#subscriptionchangeorder-newsublineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionChangeOrder-newSubLineElement

Browser definition `subscriptionChangeOrder-newSubLineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `discount` | Discount | number | double |  |  |  |
| `include` | Include | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDisplay` | Item | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `multiplierLine` | Included Quantity Multiplier | integer | int64 |  |  |  |
| `pricePlan` |  | pricePlan |  |  | [`pricePlan`](pricePlan.md#priceplan) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `required` | Required | string |  |  |  |  |
| `sequence` | Line Number | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `DRAFT` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `subscriptionLineType` |  | object |  |  |  |  |
| `subscriptionLineType.id` | Internal identifier | string |  |  |  |  |
| `subscriptionLineType.refName` | Reference Name | string |  |  |  |  |
| `upliftPercent` | % Uplift | number | double |  |  |  |

## subscriptionChangeOrder-renewalStepsCollection

Browser definition `subscriptionChangeOrder-renewalStepsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionChangeOrder-renewalStepsElement[] |  |  | [`subscriptionChangeOrder-renewalStepsElement`](#subscriptionchangeorder-renewalstepselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionChangeOrder-renewalStepsElement

Browser definition `subscriptionChangeOrder-renewalStepsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `error` | Error Message | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `SUCCESS`, `FAILURE` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `step` |  | object |  |  |  |  |
| `step.id` | Internal identifier | string |  |  |  | `CREATE_NEW_SUBSCRIPTION`, `CREATE_NEW_SALES_TRANSACTION` |
| `step.refName` | Reference Name | string |  |  |  |  |
| `subscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## subscriptionChangeOrder-subLineCollection

Browser definition `subscriptionChangeOrder-subLineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | subscriptionChangeOrder-subLineElement[] |  |  | [`subscriptionChangeOrder-subLineElement`](#subscriptionchangeorder-sublineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionChangeOrder-subLineElement

Browser definition `subscriptionChangeOrder-subLineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `apply` | Include | boolean |  |  |  |  |
| `billingMode` | Billing Mode | string |  |  |  |  |
| `discount` | Discount | number | double |  |  |  |
| `discountNew` | Discount | number | double |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `includeInRenewal` | Include In Renewal Subscription | boolean |  |  |  |  |
| `item` | Item | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `pricePlan` | Rate Plan | integer | int64 |  |  |  |
| `pricePlanNew` |  | pricePlan |  |  | [`pricePlan`](pricePlan.md#priceplan) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityNew` | Quantity | number | float |  |  |  |
| `recurringAmount` | Recurring Amount | number | double |  |  |  |
| `recurringAmountNew` | Recurring Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sequence` | Line Number | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` | Status | string |  |  |  |  |
| `statusNew` |  | object |  |  |  |  |
| `statusNew.id` | Internal identifier | string |  |  |  | `DRAFT`, `PENDING_ACTIVATION`, `ACTIVE`, `SUSPENDED`, `CLOSED` |
| `statusNew.refName` | Reference Name | string |  |  |  |  |
| `subscriptionLine` | Subscription Line | integer | int64 |  |  |  |
| `terminationDate` | Termination Date | string | date |  |  |  |
| `upliftPercent` | % Uplift | number | double |  |  |  |
| `upliftPercentNew` | % Uplift | number | double |  |  |  |

## subscriptionChangeOrderCollection

Browser definition `subscriptionChangeOrderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | subscriptionChangeOrder[] |  |  | [`subscriptionChangeOrder`](#subscriptionchangeorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## subscriptionChangeOrderSelectOptions

Browser definition `subscriptionChangeOrderSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `action` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `modificationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `renewalMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `renewalPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `renewalPriceBook` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `renewalTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `renewalTranType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `requestor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscription` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionChangeOrderStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subscriptionPlan` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
