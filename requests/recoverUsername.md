---
icon: note
tags: [requests]
title: Recover Username
---
# Recover
Sends by email the username of an account

## Method
`POST`

## Endpoint
`/account/recover_username`


## Parameters
| Name| Description |
| --- | --- |
|`forgotusername_email`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "forgotusername_email": "joe@idello.org",
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

