# Segmentation Funnels

This section covers all about creating and working with segmentation funnels.

## Create Segmentation Funnel

```shell
curl -X POST "{{BASE_URL}}/segmentation_funnels"
  -H "Accept: application/vnd.ask.v1"
  -H "Authorization: [ACCESS-TOKEN]"
  -d '{"segmentation_funnel":
  		{"name": "Funnel Name",
  		 "internal_name": "SF001",
  		 "quiz_type_id": 1
  		}
	  }'
```

> Resulting JSON

```json
{
  "data": {
    "id": "5",
    "type": "segmentation_funnels",
    "attributes": {
      "name": "Otro",
      "internal_name": "Juancho",
      "status": "draft",
      "funnel_type": "outcome",
      "wp_text": null,
      "wp_bg_image": null,
      "welcome_page": false,
      "updated_at": "Nov 02, 2016"
    },
    "relationships": {
      "quiz_type": {
        "data": {
          "id": "4",
          "type": "quiz_types"
        }
      },
      "sections": {
        "data": [
          {
            "id": "4",
            "type": "sections"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "4",
      "type": "sections",
      "attributes": {
        "name": "first"
      }
    }
  ]
}
```

### List of attributes

attribute | type | required
----------|------|---------
name | string | true
internal_name | string | false
quiz_type_id | integer | false


## List a User's Segmentation Funnels


## Change a Segmentation Funnel's Status


## Edit Segmentation Funnel


## List a Segmentation Funnel's Outcomes


## Update a Segmentation Funnel's Welcome Page


## Deactivate a Segmentation Funnel's Welcome Page

