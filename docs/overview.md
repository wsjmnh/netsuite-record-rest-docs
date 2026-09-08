# Overview

Record REST API **v1**, browser release **2026.1**.

## Base path

All operation paths in this catalog are relative to:

```
https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1
```

Example: `GET /account` is `GET https://{accountId}.suitetalk.api.netsuite.com/services/rest/record/v1/account`.

The browser dump prints the same base as `https://[accountid].suitetalk.api.netsuite.com/services/rest/record/v1`.

## Resource shapes

| Kind | Path shape | Typical methods | Notes |
| --- | --- | --- | --- |
| Collection | `/{record}` | GET, POST, PATCH, PUT, DELETE | List, insert, and batch-style updates/deletes on the record type |
| Instance | `/{record}/{id}` | GET, POST (rare), PATCH, PUT, DELETE | Single record. PUT `id` is an external identifier on upsert; other methods use an internal identifier unless noted on the operation |
| Sublist | *(none as a path)* | — | This 2026.1 browser dump has **no** `/{record}/{id}/{sublist}` operations. Sublists appear as record schema properties that `$ref` a `{record}-{sublist}Collection` / `Element` pair |
| Transform | `/{record}/{id}/!transform/{target}` | POST | Request body is the **target** record schema |
| Attach | `/{record}/{targetId}/!attach/{type}/{attachmentId}` | POST | Path ids are internal identifiers; some operations send an inline `role` object |
| Detach | `/{record}/{targetId}/!detach/{type}/{attachmentId}` | POST | Same path pattern as attach |

`{record}` is the browser tag id (same as the Markdown filename under `docs/records/`).

Not every tag exposes every collection method. See each record page for the operations that actually appear.

## Shared collection and instance parameters

These names recur across record operations. Per-record pages list which ones appear (name, in, required, type) and do not repeat the notes below.

### Query

| Name | Type | Default | Role |
| --- | --- | --- | --- |
| `q` | string | | Collection search filter |
| `limit` | integer (int32) | `1000` | Page size |
| `offset` | integer (int32) | `0` | Page offset |
| `ids` | string | | Comma-separated internal ids, or external ids with `eid:` prefix; used for batch collection operations. Marked required on collection DELETE |
| `expandRecords` | boolean | | When `true`, collection GET is a batch read of the `ids` list |
| `expandSubResources` | boolean | `false` on some operations | Expand sublists / subrecords (create/edit form and some reads) |
| `expand` | string | | Named sublists / subrecords to expand (create/edit form) |
| `fields` | string | | Field and sublist names to return |
| `replace` | string | | Comma-separated sublist names whose lines are replaced by the request body |
| `replaceSelectedFields` | boolean | `false` | When `true`, fields to clear (including body fields) must also be named in `replace` |
| `simpleEnumFormat` | boolean | | When `true`, enumerations serialize as internal id only |

### Headers

| Name | Type | Enum / default | Role |
| --- | --- | --- | --- |
| `Prefer` | string | `respond-async` | Ask the server to run the call asynchronously; async replies include `Preference-applied: respond-async` |
| `X-NetSuite-Idempotency-Key` | string | | UUID (RFC 4122) so an async call runs once; ignored when the call is synchronous. Sometimes marked required in the dump |
| `X-NetSuite-PropertyNameValidation` | string | `Error`, `Warning`, `Ignore` (default `Error` or `Warning` by operation) | How unknown property names are treated |
| `X-NetSuite-PropertyValueValidation` | string | `Error`, `Warning`, `Ignore` (default `Error`) | How invalid property values are treated |
| `Accept` | string | `application/vnd.oracle.resource+json; type=create-form`, `type=edit-form`, and/or `type=select-options` | On collection POST and instance PATCH in this dump (create-form / edit-form / select-options). Some transforms use `type=create-form` only |

### Path

| Name | Type | Role |
| --- | --- | --- |
| `id` | string or integer (int32) | Record identifier. GET/PATCH/DELETE: internal id. PUT instance: external id (upsert). Transform: internal id (int32 in the dump) |
| `targetId` | integer (int32) | Attach/detach target internal id |
| `attachmentId` | integer (int32) | Attach/detach related-record internal id |

## Media types (response labels)

Operation panels label Oracle resource media types such as `application/vnd.oracle.resource+json; type=singular`, `type=collection`, `type=error`, `type=create-form`, and `type=select-options`. Error payloads use `nsError`.

## `nsError`

Shared error body. Properties:

| Property | Label | Type | Format | Flags | Ref |
| --- | --- | --- | --- | --- | --- |
| `o:errorDetails` |  | object[] |  | read-only |  |
| `o:errorDetails[].detail` | Detail | string |  | read-only |  |
| `o:errorDetails[].o:errorCode` | Error Code | string |  | read-only |  |
| `o:errorDetails[].o:errorHeader` | Error Header | string |  | read-only |  |
| `o:errorDetails[].o:errorPath` | Error Path | string | JSONPath | read-only |  |
| `o:errorDetails[].o:errorQueryParam` | Error Query Parameter | string |  | read-only |  |
| `o:errorDetails[].o:errorUrl` | Error URL | string | URI | read-only |  |
| `status` | Status | integer | int32 | read-only |  |
| `title` | Title | string |  | read-only |  |
| `type` | Type | string | URI | read-only |  |

Related shared schemas: [`nsLink`](schemas/ns.md#nslink), [`nsResource`](schemas/ns.md#nsresource), [`nsResourceCollection`](schemas/ns.md#nsresourcecollection), [`nsResourceSelectOptions`](schemas/ns.md#nsresourceselectoptions).
