---
icon: note
tags: [requests]
---
# Sign up
Create a new account

## Method
`POST`

## Endpoint
`/account/signup`

## Parameters
| Name| Description |
| --- | --- |
|`username`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"]
|`password`| [!badge text="string" variant="light"] [!badge text="min_length(8)" variant="light"] [!badge text="required" variant="warning"] 
|`password_confirm`| [!badge text="string" variant="light"] [!badge text="min_length(8)" variant="light"] [!badge text="required" variant="warning"] Must match `password`
|`type`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Accepted value: ‘child’, ‘student’, ‘parent’, ‘teacher’, ‘manager’ 
|`birthyear`| [!badge text="string" variant="light"] [!badge text="length(4)" variant="light"] [!badge text="required" variant="warning"] 
|`firstname`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 
|`lastname`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 
|`email`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 
|`institution_id`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Groupe Media TFO = 1435
|`lang`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Accepted value: 'en', 'fr'
|`country_destination_id`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Canada = 40
|`region_destination_id`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Ontario = 922
|`conditions_accepted`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] User must accept conditions
|`g-recaptcha-response`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] ReCaptcha challenge's response
|`receive_newsletter`| [!badge text="string" variant="light"] Define if the user want to subscribe to Idello newsletter
|`receive_newsletter_tfo`| [!badge text="string" variant="light"] Define if the user want to subscribe to TFO newsletter

Example
```
{
  "username": "string",
  "password": "string",
  "password_confirm": "string",
  "invitation_token": "string",
  "group_token": "string",
  "promo_token": "string",
  "type": "string",
  "birthyear": 0,
  "firstname": "string",
  "lastname": "string",
  "email": "string",
  "institution_id": "string",
  "lang": "string",
  "province": "string",
  "country_destination_id": "string",
  "region_destination_id": "string",
  "receive_newsletter": 0,
  "receive_newsletter_tfo": 0,
  "receive_newsletter_partners": 0,
  "conditions_accepted": 0,
  "security_question": 0,
  "security_answer": 0
  "g-recaptcha-response": "string
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
    "session_name": "X-tfo-idello-session",
    "session_id": "xyz1234"
  }
}
```


| Name| Description |
| --- | --- |
|`session_name`| Session name, used for setting POST headers
|`session_id`| Session ID for subsequent calls