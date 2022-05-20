---
icon: note
tags: [algolia]
---
# Generate API Key List
Get a new api key to make direct request to Algolia from the frontend

## Method
`POST`

## Endpoint
`/algolia/generateApiKey`

## Parameters
| Name| Description |
| --- | --- |
|`scope`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Value must be `idello`
|`refresh`| [!badge text="boolean" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "scope": "idello",
  "refresh": false,
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
    "key": "string",
    "appId": "string",
    "defaultIndexName": "string",
    "indices": {}
  }
}
```

