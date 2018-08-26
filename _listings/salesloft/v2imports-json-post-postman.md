{
  "info": {
    "name": "SalesLoft Create an import",
    "_postman_id": "0207b4aa-7169-4a72-9097-872067a03668",
    "description": "Creates an import.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sales",
      "item": [
        {
          "id": "c8759e67-48eb-45d0-8e5e-8bdc51879f11",
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
              "id": "d3296f78-5f6b-4496-ab44-d500c33084ff"
            }
          ]
        },
        {
          "id": "cd9f331c-e0a1-4fc3-971e-d37ceac5fdd3",
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
              "id": "f6b67792-93fe-4007-a43c-1de2b8d3d33e"
            }
          ]
        },
        {
          "id": "268590d8-055e-437d-b587-e09399fc5263",
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
              "id": "df83e658-77fc-4416-af5e-655046e903d7"
            }
          ]
        },
        {
          "id": "908b3c8d-e926-4c9a-9e3b-ea27b7b54e95",
          "name": "v2.accounts.id.json.put",
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
            "method": "PUT",
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
            "description": "Updates an account.\n\n\"domain\" must be unique on the current team."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a327813-f29e-4ab3-a18c-8dfa023e0489"
            }
          ]
        },
        {
          "id": "0e8cbe77-5fc0-4b39-9482-fa69915a7da6",
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
              "id": "b0130b46-706a-43b6-a781-7936b5bfcae9"
            }
          ]
        },
        {
          "id": "f3f2578e-fb16-4392-8265-399155dfe4f3",
          "name": "v2.action_details.call_instructions.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/action_details/call_instructions.json?ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D",
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
            "description": "Fetches multiple call instruction records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b44986e-00f6-4090-8be1-5418e3ef809b"
            }
          ]
        },
        {
          "id": "2e9846b0-52a7-41d9-bd56-e58713771610",
          "name": "v2.action_details.call_instructions.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/action_details/call_instructions/:id.json"
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
            "description": "Fetches a call instruction, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce8a3ec7-86a2-4758-b930-cfc470742fc4"
            }
          ]
        },
        {
          "id": "14c7928c-b2ee-4c3c-ac15-35fc91e9101b",
          "name": "v2.actions.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/actions.json?due_on=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&step_id=%7B%7D&type=%7B%7D",
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
            "description": "Fetches multiple action records. The records can be filtered, paged, and sorted according to\nthe respective parameters. Only actions that are currently \"in_progess\" will be returned by\nthis endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66c41f55-f5a8-4cea-92f3-5add7ca7704a"
            }
          ]
        },
        {
          "id": "d7ef73d3-5889-479b-9fee-b63649a76248",
          "name": "v2.actions.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/actions/:id.json"
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
            "description": "Fetches an action, by ID only.\nThis endpoint will only return actions that are in_progress or pending_activity.\nOnce an action is complete, the request for that action will return a 404 status code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33c0d210-3b7d-4133-a41e-466fdf89563a"
            }
          ]
        },
        {
          "id": "69356fe6-cce6-4f8e-b9c0-218a64b4fe23",
          "name": "v2.activities.calls.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/activities/calls.json?ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple call records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26377730-6838-450d-bec1-7b135561c655"
            }
          ]
        },
        {
          "id": "d1eb7f2c-210f-4bf7-8afd-8816cd2da42f",
          "name": "v2.activities.calls.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/activities/calls/:id.json"
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
            "description": "Fetches a call, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af4e3b69-dc95-467e-9563-84ccdafb1d7d"
            }
          ]
        },
        {
          "id": "074694f0-6e76-4861-990a-0c43331fc193",
          "name": "v2.activities.emails.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/activities/emails.json?bounced=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple email records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "908bb94b-e13e-4d77-b43f-983bdc8d50f2"
            }
          ]
        },
        {
          "id": "d52c62ca-b294-4386-987e-f1ca2160775c",
          "name": "v2.activities.emails.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/activities/emails/:id.json"
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
            "description": "Fetches an email, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ce6d834-8f09-4970-94f3-33560b0a6437"
            }
          ]
        },
        {
          "id": "d22b8432-2a36-46bb-95c0-b900c7d19921",
          "name": "v2.cadence_memberships.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/cadence_memberships.json?cadence_id=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&person_id=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple cadence membership records. The records can be filtered, paged, and sorted according to\nthe respective parameters. A cadence membership is the association between a person and their current and\nhistorical time on a cadence. Cadence membership records are mutable and change over time. If a person is\nadded to a cadence and re-added to the same cadence in the future, there is a single membership record."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f6199ea-5af4-4d38-a0f9-512297612709"
            }
          ]
        },
        {
          "id": "52340497-4b49-4d15-9802-81ea2f2f39c4",
          "name": "v2.cadence_memberships.json.post",
          "request": {
            "url": "http://api.salesloft.com/v2/cadence_memberships.json?cadence_id=%7B%7D&person_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
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
            "description": "Adds a person to a cadence. person_id and cadence_id are required, and must be visible to the authenticated user. user_id will\ndefault to the authenticated user, but can be set to any visible user on the authenticated team.\n\nA person cannot be added to a cadence on behalf of a teammate unless the cadence is a team cadence, or the cadence is owned by\nthe teammate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a87b7e5f-262b-4adc-9c24-d71e3333b855"
            }
          ]
        },
        {
          "id": "8428f414-cc55-4d01-b898-4c4072eb5643",
          "name": "v2.cadence_memberships.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/cadence_memberships/:id.json"
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
            "description": "Fetches a cadence membership, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9bdc647-df38-4ae7-9152-b9bd1d22ab8d"
            }
          ]
        },
        {
          "id": "51a709ad-e0bb-410e-83fd-df4d4e5dc969",
          "name": "v2.cadence_memberships.id.json.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/cadence_memberships/:id.json"
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
            "description": "Delete a cadence membership"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e507d8c2-7bbc-4609-92cf-d328f1b8d3b2"
            }
          ]
        },
        {
          "id": "1882f2b5-7f21-4829-827e-7590753424cd",
          "name": "v2.cadences.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/cadences.json?ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&team_cadence=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple cadence records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c914cd4-6894-4b55-81e1-92b2da70d400"
            }
          ]
        },
        {
          "id": "1a31c0dd-3897-4dd3-8f55-0cd8f688e725",
          "name": "v2.cadences.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/cadences/:id.json"
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
            "description": "Fetches a cadence, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "161920df-5633-4c1d-b56d-bc4f6a3c66f8"
            }
          ]
        },
        {
          "id": "01ada218-e3e3-40d9-96bd-fe0c9f30b743",
          "name": "v2.call_data_records.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/call_data_records.json?has_call=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple call data records. The records can be filtered, paged, and sorted according to\nthe respective parameters.\n\nCall data records are records of all inbound and outbound calls through SalesLoft. A call data record may\nbe associated with a call, but does not have to be."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80400e9e-d60e-46de-b08b-bf3bda55ed41"
            }
          ]
        },
        {
          "id": "32df4510-3fd3-4cbc-9c1d-4f92c8af4571",
          "name": "v2.call_data_records.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/call_data_records/:id.json"
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
            "description": "Fetches a call data record, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09b6dcfa-3adb-42e1-aa78-1a2b727059ff"
            }
          ]
        },
        {
          "id": "8aec36a4-2c6c-4bef-9629-f7e814f67cd2",
          "name": "v2.crm_activities.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/crm_activities.json?ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple crm activity records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c57faf6-d496-4ae2-a918-91b1cc59bc84"
            }
          ]
        },
        {
          "id": "385970f5-06c8-4d7f-a4f1-d53f09eaa1c4",
          "name": "v2.crm_activities.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/crm_activities/:id.json"
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
            "description": "Fetches a crm activity, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a31ac7d1-63e6-4974-abfb-707351444f03"
            }
          ]
        },
        {
          "id": "2cbfdd0e-9da0-4a50-81c9-84c9ae806e09",
          "name": "v2.custom_fields.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/custom_fields.json?field_type=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D",
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
            "description": "Fetches multiple custom field records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "490ce1e1-fea2-4386-a90e-0568dcc27ce4"
            }
          ]
        },
        {
          "id": "cf2c6dee-f2b0-42eb-b56c-602ca1bfb6ee",
          "name": "v2.custom_fields.json.post",
          "request": {
            "url": "http://api.salesloft.com/v2/custom_fields.json",
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
                  "key": "field_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "The field type of the custom field"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the custom field"
                }
              ]
            },
            "description": "Creates a custom field."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26caddad-236f-4920-8053-ad8685201dc5"
            }
          ]
        },
        {
          "id": "df730866-6026-4b5f-bda3-5f4569815992",
          "name": "v2.custom_fields.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/custom_fields/:id.json"
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
            "description": "Fetches a custom field, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35c3b15a-2c37-4531-ae19-f30c20898c23"
            }
          ]
        },
        {
          "id": "56d01146-ac19-4a1b-a9b3-c0a57491876b",
          "name": "v2.custom_fields.id.json.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/custom_fields/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "field_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "The field type of the custom field"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the custom field"
                }
              ]
            },
            "description": "Update a custom field."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "731bb419-b465-4baa-818d-ae6afcc31a92"
            }
          ]
        },
        {
          "id": "6b75c053-e258-4937-9a1c-0c2e514588e5",
          "name": "v2.custom_fields.id.json.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/custom_fields/:id.json"
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
            "description": "Deletes a custom field."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d0ee09e-72ec-4658-8a79-fbb5edf40e8a"
            }
          ]
        },
        {
          "id": "940dc182-5291-4f44-8764-089d2590b499",
          "name": "v2.email_templates.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/email_templates.json?ids=%7B%7D&include_paging_counts=%7B%7D&linked_to_team_template=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple email template records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a64b75b-58f9-419d-a2a9-303ff3047f7b"
            }
          ]
        },
        {
          "id": "c3106a6f-8e78-48cc-86d9-e6ae73c6400a",
          "name": "v2.email_templates.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/email_templates/:id.json"
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
            "description": "Fetches an email template, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1aa62f46-db6b-4c54-8e1a-3d84c6817876"
            }
          ]
        },
        {
          "id": "18992647-ccff-47f1-82e3-da449bbd1cfc",
          "name": "v2.imports.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/imports.json?ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&user_ids=%7B%7D",
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
            "description": "Fetches multiple imports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "052f10df-5f7d-4893-977d-36e795026098"
            }
          ]
        },
        {
          "id": "380e8be6-91b8-46ad-a60c-b0c93cbbaf4f",
          "name": "v2.imports.json.post",
          "request": {
            "url": "http://api.salesloft.com/v2/imports.json",
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
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Name, recommended to be easily identifiable to a user"
                },
                {
                  "key": "user_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the User that owns this Import"
                }
              ]
            },
            "description": "Creates an import."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c7b995f-6635-4e04-8bce-e0ced882e516"
            }
          ]
        }
      ]
    }
  ]
}