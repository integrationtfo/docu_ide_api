---
icon: note
tags: [requests]
title: Check Username
---
# Recover
Retrieve security question, providing username. Useful in password recovery flow without an email

## Method
`POST`

## Endpoint
`/account/check_username`


## Parameters
| Name| Description |
| --- | --- |
|`noemail_username`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "noemail_username": "joe2",
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
    "username": "joe2",
    "question": "joe2",
    "tries_left": 3
  }
}
```

