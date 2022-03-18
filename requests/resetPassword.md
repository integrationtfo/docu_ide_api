---
icon: note
tags: [requests]
---
# Reset Password
Get a link to reset password

## Method
`POST`

## Endpoint
`/account/validate_security_question_answer`


## Parameters
| Name| Description |
| --- | --- |
|`noemail_username`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 
|`noemail_secretquestion`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "noemail_username": "joe",
  "noemail_secretquestion": "My answer"
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
    "recover_link": "string"
  }
}
```

