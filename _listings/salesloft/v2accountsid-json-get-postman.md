{
  "info": {
    "name": "SalesLoft Fetch an account",
    "_postman_id": "0ab918d3-4b0a-42fd-a4bf-fcdaa2b7883c",
    "description": "Fetches an account, by ID only.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sales",
      "item": [
        {
          "id": "0b2dc89b-6d90-4c36-be92-3dbac0549e63",
          "name": "v2.accounts.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/accounts.json?domain=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Fetches multiple account records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f5a2c70-f063-4d45-a62c-0de3aa0ad2ad"
            }
          ]
        },
        {
          "id": "37e82010-9e41-4bde-b33d-12b57933d4cf",
          "name": "v2.accounts.json.post",
          "request": {
            "url": "http://api.salesloft.com/v2/accounts.json",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": "City"
                },
                {
                  "key": "company_stage_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the CompanyStage assigned to this Account"
                },
                {
                  "key": "company_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Type of the Accounts company"
                },
                {
                  "key": "conversational_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Conversational name of the Account"
                },
                {
                  "key": "country",
                  "value": "{}",
                  "disabled": false,
                  "description": "Country"
                },
                {
                  "key": "custom_fields",
                  "value": "{}",
                  "disabled": false,
                  "description": "Custom fields are defined by the users team"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "Description"
                },
                {
                  "key": "domain",
                  "value": "{}",
                  "disabled": false,
                  "description": "Website domain, not a fully qualified URI"
                },
                {
                  "key": "do_not_contact",
                  "value": "{}",
                  "disabled": false,
                  "description": "Whether this company can not be contacted"
                },
                {
                  "key": "founded",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date or year of founding"
                },
                {
                  "key": "industry",
                  "value": "{}",
                  "disabled": false,
                  "description": "Industry"
                },
                {
                  "key": "linkedin_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Full LinkedIn url"
                },
                {
                  "key": "locale",
                  "value": "{}",
                  "disabled": false,
                  "description": "Time locale"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Account Full Name"
                },
                {
                  "key": "owner_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the User that owns this Account"
                },
                {
                  "key": "phone",
                  "value": "{}",
                  "disabled": false,
                  "description": "Phone number without formatting"
                },
                {
                  "key": "postal_code",
                  "value": "{}",
                  "disabled": false,
                  "description": "Postal code"
                },
                {
                  "key": "revenue_range",
                  "value": "{}",
                  "disabled": false,
                  "description": "Estimated revenue range"
                },
                {
                  "key": "size",
                  "value": "{}",
                  "disabled": false,
                  "description": "Estimated number of people in employment"
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": "State"
                },
                {
                  "key": "street",
                  "value": "{}",
                  "disabled": false,
                  "description": "Street name and number"
                },
                {
                  "key": "tags",
                  "value": "{}",
                  "disabled": false,
                  "description": "All tags applied to this Account"
                },
                {
                  "key": "twitter_handle",
                  "value": "{}",
                  "disabled": false,
                  "description": "Twitter handle, with @"
                },
                {
                  "key": "website",
                  "value": "{}",
                  "disabled": false,
                  "description": "Website"
                }
              ]
            },
            "description": "Creates an account.\n\n\"domain\" must be unique on the current team."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "021a5b61-9c54-42f9-b0e0-ee0608dc5fce"
            }
          ]
        },
        {
          "id": "6a559b25-5752-4d64-9499-f8d67913315c",
          "name": "v2.accounts.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/accounts/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Fetches an account, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e562221-defc-457e-8304-40ddf7f52830"
            }
          ]
        },
        {
          "id": "40e6c1fd-33cd-44b6-b9d0-06be4f0121ca",
          "name": "v2.accounts.id.json.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/accounts/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an account. This operation is not reversible without contacting support.\nThis operation can be called multiple times successfully.\n\nDeleting an account will remove all connected people from that account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5864ce84-23ae-45c5-880d-bb0a54a52af8"
            }
          ]
        }
      ]
    }
  ]
}