---
icon: note
tags: [requests]
---
# Get Countries List
Get list of provinces with codes and id.

## Method
`POST`

## Endpoint
`/account/get_provinces_list`

## Parameters
| Name| Description |
| --- | --- |
|`country_id`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "country_id": 40,
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
  "data": [
    {
      "id": 1,
      "title": "Ontario",
      "code": "on"
    }
  ]
}
```

