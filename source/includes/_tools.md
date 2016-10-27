# Utilities

This section covers utilities endpoints which, mostly, do not require an `access token` to be requested.

## Recover Password

```shell
curl -X POST "{{BASE_URL}}/tools/recover_password"
  -H "Accept: application/vnd.ask.v1"
  -d '{"email": "c1@email.com"}'
```

> Results in

```json
{
  "message": "Reset instructions sent to c1@email.com"
}
```

### HTTP Request

`POST {{BASE_URL}}/tools/recover_password`

### Query Parameters

Parameter | Description
--------- | -----------
email *(string)* | The user's email address


## Reset Password

```shell
curl -X PUT "{{BASE_URL}}/tools/reset-password"
  -H "Accept: application/vnd.ask.v1"
  -d '{"tool":
  		{"reset_password_token": "oPTiLgvif6nDqz7p1vZD",
  		 "password": "123456789",
  		 "password_confirmation": "123456789"}
	  }'
```

> Results in

```json
{
  "message": "Password updated"
}
```

### HTTP Request

`PUT {{BASE_URL}}/tools/reset-password`

### Query Parameters

Parameter | Description
--------- | -----------
tool *(object)* | An object that contains the values to change the password
reset_password_token *(string)* | Token sent in the `{{BASE_URL}}/tools/recover_password`
password *(string)* | New user's password
password_confirmation *(string)* | Confirmation of the new password

