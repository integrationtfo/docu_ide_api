---
icon: note
tags: [requests]
---
# Recover Password
Recover account password using slug and code sent by mail

## Method
`POST`

## Endpoint
`/account/recover_password`


## Parameters
| Name| Description |
| --- | --- |
|`slug`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 
|`code`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 
|`password`| [!badge text="string" variant="light"] [!badge text="min_length(8)" variant="light"] [!badge text="required" variant="warning"] 
|`password_confirm`| [!badge text="string" variant="light"] [!badge text="min_length(8)" variant="light"] [!badge text="required" variant="warning"] Must match `password` 

Example
```
{
  "slug": "string",
  "code": "string",
  "password": "string",
  "password_confirm": "string"
}
```

## Responses

Example
```
# Code 200
{
  "success": 1,
  "msg": "OK",
  "code": "OK"
}
```

