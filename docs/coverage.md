# Coverage

Parsed from the Spectacle dump at [https://system.netsuite.com/help/helpcenter/en_US/APIs/REST_API_Browser/record/v1/2026.1/index.html](https://system.netsuite.com/help/helpcenter/en_US/APIs/REST_API_Browser/record/v1/2026.1/index.html) (chunks `data00.part`–`data27.part`).

## Counts

| Item | Count |
| --- | ---: |
| Record tags (`id=tag-*`) | 206 |
| Operation panels | 1961 |
| Schema definitions | 1905 |
| Schema properties (including nested) | 29571 |
| Unique operation paths | 541 |

### HTTP methods

| Method | Operations |
| --- | ---: |
| DELETE | 398 |
| GET | 411 |
| PATCH | 410 |
| POST | 330 |
| PUT | 412 |

### Path kinds

| Kind | Operations |
| --- | ---: |
| attach | 33 |
| collection | 1016 |
| detach | 33 |
| instance | 816 |
| transform | 63 |

## Completeness

- Tags with at least one operation: 206 / 206
- Tags with zero operations: 0
- Schema panels that failed property parse: 0
- Schema panels with zero properties: 0

Every parsed tag has an operations list.

Every schema definition panel was parsed for properties.

## Source files

- Index: https://system.netsuite.com/help/helpcenter/en_US/APIs/REST_API_Browser/record/v1/2026.1/index.html
- Chunks: `chunks/data00.part` through `chunks/data27.part` (same directory as the index)

## What was extracted

- Tag ids, operation method/path/id/one-line summary, parameters (name, in, required, type/format/enum/default), request `$ref` or inline property names, response status + `$ref`
- Schema definition ids and property tables (name, label, type, format, flags, ref, enum values)

## What was not copied

- Oracle/Spectacle description paragraphs (`<dd>` help text, long parameter blurbs)
- Account-specific custom records/fields (not in this public browser dump)
