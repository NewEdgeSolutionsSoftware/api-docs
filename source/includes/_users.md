# Users

## Create Account

```shell
curl -X POST "{{BASE_URL}}/users"
  -H "Accept: application/vnd.ask.v1"
  -d '{"user":
  		{"email": "c1@email.com", "password": "123456789"}
	  }'
```

> Result JSON

```json
{
  "data": {
    "id": "2",
    "type": "users",
    "attributes": {
      "access_token": "nprH_L7zqdzzuYwRox1N",
      "email": "c2@email.com",
      "full_name": null
    }
  }
}
```

This endpoint creates a new user account with the given credentials.

<aside class="warning">
	Notice this endpoint does not requires an <code>access-token</code>
</aside>

### HTTP Request

`POST {{BASE_URL}}/users`

### Query Parameters

Parameter | Description
--------- | -----------
user *(object)* | An object that contains the email and password values
email *(string)* | The user's email address
password *(string)* | The user's password

