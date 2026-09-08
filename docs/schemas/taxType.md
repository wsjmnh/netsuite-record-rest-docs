# Schemas: taxType

Property tables for definitions owned by `taxType`.

Record page: [taxType](../records/taxType.md).

## Index

- [taxType](#taxtype) — 18 properties
- [taxType-nexusAccountsCollection](#taxtype-nexusaccountscollection) — 6 properties
- [taxType-nexusAccountsElement](#taxtype-nexusaccountselement) — 5 properties
- [taxType-nexusesTaxCollection](#taxtype-nexusestaxcollection) — 6 properties
- [taxType-nexusesTaxElement](#taxtype-nexusestaxelement) — 6 properties
- [taxTypeCollection](#taxtypecollection) — 6 properties
- [taxTypeSelectOptions](#taxtypeselectoptions) — 2 properties

## taxType

Browser definition `taxType`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `country` |  | object |  |  |  |  |
| `country.id` | Internal identifier | string |  |  |  | `BR`, `AU`, `SG`, `JP`, `GB`, `IT`, `FR`, `CA`, `US` |
| `country.refName` | Reference Name | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `doesNotAddToTotal` | Does Not Add to Transaction Total | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `nexusAccounts` |  | taxType-nexusAccountsCollection |  |  | [`taxType-nexusAccountsCollection`](#taxtype-nexusaccountscollection) |  |
| `nexusesTax` |  | taxType-nexusesTaxCollection |  |  | [`taxType-nexusesTaxCollection`](#taxtype-nexusestaxcollection) |  |
| `postToItemCost` | Post to Item Cost | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reverseCharge` | Reverse Charge | boolean |  |  |  |  |
| `taxInNetAmount` | Tax Included in Net Amount | boolean |  |  |  |  |
| `taxType` | Tax Type | string |  |  |  |  |

## taxType-nexusAccountsCollection

Browser definition `taxType-nexusAccountsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | taxType-nexusAccountsElement[] |  |  | [`taxType-nexusAccountsElement`](#taxtype-nexusaccountselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## taxType-nexusAccountsElement

Browser definition `taxType-nexusAccountsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `payablesAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `receivablesAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `refName` | Reference Name | string |  |  |  |  |

## taxType-nexusesTaxCollection

Browser definition `taxType-nexusesTaxCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | taxType-nexusesTaxElement[] |  |  | [`taxType-nexusesTaxElement`](#taxtype-nexusestaxelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## taxType-nexusesTaxElement

Browser definition `taxType-nexusesTaxElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `purchTaxAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `saleTaxAcct` |  | account |  |  | [`account`](account.md#account) |  |

## taxTypeCollection

Browser definition `taxTypeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | taxType[] |  |  | [`taxType`](#taxtype) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## taxTypeSelectOptions

Browser definition `taxTypeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `country` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
