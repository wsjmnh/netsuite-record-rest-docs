# Schemas: fairValueFormula

Property tables for definitions owned by `fairValueFormula`.

Record page: [fairValueFormula](../records/fairValueFormula.md).

## Index

- [fairValueFormula](#fairvalueformula) — 9 properties
- [fairValueFormulaCollection](#fairvalueformulacollection) — 6 properties
- [fairValueFormulaSelectOptions](#fairvalueformulaselectoptions) — 1 properties

## fairValueFormula

Browser definition `fairValueFormula`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fairValueFormula` | Fair Value Formula | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## fairValueFormulaCollection

Browser definition `fairValueFormulaCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | fairValueFormula[] |  |  | [`fairValueFormula`](#fairvalueformula) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## fairValueFormulaSelectOptions

Browser definition `fairValueFormulaSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
