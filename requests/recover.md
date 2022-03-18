---
icon: note
tags: [requests]
title: Recover
---
# Recover
Send recovered password email to user

## Method
`POST`

## Endpoint
`/account/recover`


## Parameters
| Name| Description |
| --- | --- |
|`email`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "email": "string",
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

