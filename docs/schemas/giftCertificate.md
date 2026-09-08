# Schemas: giftCertificate

Property tables for definitions owned by `giftCertificate`.

Record page: [giftCertificate](../records/giftCertificate.md).

## Index

- [giftCertificate](#giftcertificate) — 16 properties
- [giftCertificateCollection](#giftcertificatecollection) — 6 properties
- [giftCertificateSelectOptions](#giftcertificateselectoptions) — 2 properties

## giftCertificate

Browser definition `giftCertificate`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amountRemaining` | Amount Remaining | number | double |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `email` | Recipient Email | string |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `giftCertCode` | Code | string |  |  |  |  |
| `giftCertItem` |  | giftCertificateItem |  |  | [`giftCertificateItem`](giftCertificateItem.md#giftcertificateitem) |  |
| `id` | Internal ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `message` | Gift Message | string |  |  |  |  |
| `name` | Recipient Name | string |  |  |  |  |
| `originalAmount` | Original Amount | number | double |  |  |  |
| `purchaseDate` | Purchase Date | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sender` | From | string |  |  |  |  |

## giftCertificateCollection

Browser definition `giftCertificateCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | giftCertificate[] |  |  | [`giftCertificate`](#giftcertificate) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateSelectOptions

Browser definition `giftCertificateSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `giftCertItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
