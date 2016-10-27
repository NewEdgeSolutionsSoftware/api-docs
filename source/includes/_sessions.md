# Sessions

## Log In

```shell
curl -X POST "{{BASE_URL}}/sessions"
  -H "Authorization: [ACCESS-TOKEN]"
  -H "Accept: application/vnd.ask.v1"
  -d '{"session":
  		{"email": "c1@email.com", "password": "123456789"}
	  }'
```

> Result JSON

```json
{
  "data": {
    "id": "1",
    "type": "users",
    "attributes": {
      "access_token": "pdTFgmeAuua-VLjxRtzx",
      "email": "c1@email.com",
      "full_name": null
    }
  }
}
```

This endpoint logs in a user.

### HTTP Request

`POST {{BASE_URL}}/sessions`

### Query Parameters

Parameter | Description
--------- | -----------
sessions *(object)* | An object that contains the email and password values
email *(string)* | The user's email address
password *(string)* | The user's password


## Log Out

```shell
curl -X DELETE "{{BASE_URL}}/sessions"
  -H "Authorization: [ACCESS-TOKEN]"
  -H "Accept: application/vnd.ask.v1"
```

This endpoint logs out a user.

### HTTP Request

`DELETE {{BASE_URL}}/sessions`

<aside class="notice">
	The log out endpoint does not return a JSON but a 204 or no content status
</aside>

