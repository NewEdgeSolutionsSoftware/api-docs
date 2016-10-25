# Sessions

## Log In

```shell
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

> Result:

```json

```

This endpoint logs in a user.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

## Log Out

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

> Result:

```json

```

This endpoint logs out a user.

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

