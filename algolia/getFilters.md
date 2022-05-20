---
icon: note
tags: [algolia]
---
# Get Filters
Return algolias for a province

## Method
`POST`

## Endpoint
`/algolia/getFilters`

## Parameters
| Name| Description |
| --- | --- |
|`scope`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Value must be `idello`

Example
```
{
  "scope": "idello",
}
```


## Responses

Example
```
# Code 200
{
  "success": 1,
  "msg": "OK",
  "code": "OK",
  "data": {
    "refinementHierarchy": {}
  }
}
```

