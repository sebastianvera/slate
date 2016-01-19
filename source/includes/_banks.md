# Banks

## Get All Banks

```shell
curl "https://app.finciero.com/api/banks"
  -H "Authorization: Token token=api-token"
  -H "Accept: application/vnd.finciero+json; version=1"
```

> The above command returns JSON structured like this:

```json
{
  "data": [
    {
      "id": 7,
      "name": "Santander",
      "status": "active",
      "updated_at": "2014-02-19T01:54:02.961Z",
      "time_zone": "Santiago"
    },
    {
      "id": 10,
      "name": "Scotiabank",
      "status": "on_development",
      "updated_at": "2014-02-19T01:54:03.014Z",
      "time_zone": "Santiago"
    },
    {
      "id": 13,
      "name": "Banco Security",
      "status": "idle",
      "updated_at": "2015-04-24T21:40:05.247Z",
      "time_zone": "Santiago"
    },
    {
      "id": 16,
      "name": "HSBC Bank",
      "status": "on_maintenance",
      "updated_at": "2014-02-19T01:54:03.134Z",
      "time_zone": "Santiago"
    }
  ]
}
```

This endpoint retrieves all banks.

### HTTP Request

`GET http://app.finciero.com/api/banks`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Isis",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">If you're not using an administrator API key, note that some kittens will return 403 Forbidden if they are hidden for admins only.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve
