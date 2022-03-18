---
icon: note
tags: [requests]
---
# Get Countries List
Get list of countries with codes and id.

## Method
`POST`

## Endpoint
`/account/get_country_list`

## Responses

Example
```
# Code 200
{
  "success": 1,
  "data": [
    {
      "id": "40",
      "title": "Canada ",
      "code": "CA"
    }
  ],
  "code": "OK",
  "msg": "OK"
}
```

