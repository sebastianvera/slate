# Ads
The ads description

## Create an ad
This endpoint is awesome

### HTTP Request
`POST api/ads`

### Parameters

Name | Type | Required | Description
--------- | ------- | :-----------: | -------
ad_group_id | integer |  *  | Id of the parent group
specialization_type | string |  *  | Type of the specialization `[FormAd, LinkAd]`
name | string |  *  | Name of the ad
default_example | boolean |  | Test default values


```json
{
  "data": {
    "id": 1510,
    "specialization_id": 1423,
    "specialization_type": "FormAd",
    "ad_group_id": 1339,
    "specialization": {
      "id": 1423,
      "image_attached": {
        "content_type": "image/png",
        "file_size": 29346,
        "file_name": "test.png",
        "updated_at": "2016-01-16T23:56:25.326Z",
        "large_url": "/system/form_ads/images/000/001/423/large/test.png?1452988585",
        "thumb_url": "/system/form_ads/images/000/001/423/thumb/test.png?1452988585"
      },
      "name": "name1",
      "description": "description1",
      "email": "foo@email.com",
      "fields": [
        {
          "id": 1881,
          "name": "field_6",
          "hint": "user_email",
          "response_type": "EmailFieldResponse",
          "created_at": "2016-01-16T23:56:24.984Z",
          "updated_at": "2016-01-16T23:56:24.984Z"
        },
        {
          "id": 1882,
          "name": "field_7",
          "hint": "user_email",
          "response_type": "EmailFieldResponse",
          "created_at": "2016-01-16T23:56:25.248Z",
          "updated_at": "2016-01-16T23:56:25.248Z"
        },
        {
          "id": 1883,
          "name": "field_8",
          "hint": "user_email",
          "response_type": "EmailFieldResponse",
          "created_at": "2016-01-16T23:56:25.293Z",
          "updated_at": "2016-01-16T23:56:25.293Z"
        },
        {
          "id": 1884,
          "name": "field_9",
          "hint": "user_email",
          "response_type": "EmailFieldResponse",
          "created_at": "2016-01-16T23:56:25.298Z",
          "updated_at": "2016-01-16T23:56:25.298Z"
        }
      ]
    }
  }
}
`
