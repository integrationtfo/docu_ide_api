---
icon: note
tags: [requests]
---
# Sign out

## Method
`POST`

## Endpoint
`/account/signout`

## Parameters
| Name| Description |
| --- | --- |
|`X-tfo-idello-session`| [!badge text="string (header)" variant="light"] [!badge text="required" variant="warning"]
|`password`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] md5 hash of the user password


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
