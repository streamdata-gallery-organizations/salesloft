{
  "info": {
    "name": "SalesLoft Create a person stage",
    "_postman_id": "593d08af-1d71-4f3e-bfcb-57e2d8d28950",
    "description": "Creates a person stage.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sales",
      "item": [
        {
          "id": "8fd6761b-1945-480f-86b6-ed40b47319ad",
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
              "id": "195b8ef9-e71c-440e-8866-c4aebe0f48a6"
            }
          ]
        },
        {
          "id": "ece71be1-641c-497b-961e-06608a34816d",
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
              "id": "41bbd952-d361-4adf-9d4d-a51639f6557f"
            }
          ]
        },
        {
          "id": "8c4bfca5-e0bb-4ac3-bce0-46f25d46150f",
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
              "id": "4d0bdb86-a024-4931-86e2-da9f576e6640"
            }
          ]
        },
        {
          "id": "9668a170-1e11-4df4-8e82-28a246083996",
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
              "id": "201bff02-a226-4f0c-b654-5d8b7b03d128"
            }
          ]
        },
        {
          "id": "4be9e9c1-7196-413a-b26e-81ff6b8939c9",
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
              "id": "f619ce89-4dae-41b4-8b8e-3b713be95b32"
            }
          ]
        },
        {
          "id": "f1b8f0cd-5527-4dcc-9bea-a2dd1b81b08f",
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
              "id": "17723c6f-76fc-425a-88f2-fa3629beb545"
            }
          ]
        },
        {
          "id": "93a5cff0-6025-4142-8829-9e14a86010d3",
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
              "id": "470b1b9e-cea4-4d7f-ab3d-1784ffafe562"
            }
          ]
        },
        {
          "id": "4f53577f-79cc-4629-8565-646153963408",
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
              "id": "88b96015-3aeb-4577-b0ec-3b6502cca25f"
            }
          ]
        },
        {
          "id": "2cfac180-2623-44bc-b08e-d96a6c78fc1a",
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
              "id": "3ea6d493-d35a-4f14-943b-a807ec67615d"
            }
          ]
        },
        {
          "id": "bfc9bcff-e4bd-4b9b-a522-c50fdd01a02c",
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
              "id": "d6764b42-63da-49f7-a725-e42c27e1bbb7"
            }
          ]
        },
        {
          "id": "610c036a-f9bc-49a1-aeb5-88bd601e2c79",
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
              "id": "03d75a35-be06-486e-ac54-c973fd6ec613"
            }
          ]
        },
        {
          "id": "99c4d27b-51c6-4f86-a221-be2cc037640b",
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
              "id": "bdee5e00-5157-4b13-bde2-49233caa6a9c"
            }
          ]
        },
        {
          "id": "a214553a-c04b-45b6-875e-66869aae60bb",
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
              "id": "8cecac4a-2801-475f-8e48-3b328005f1fb"
            }
          ]
        },
        {
          "id": "f4cf0a40-1777-4fd9-8b0f-dbe6a221afa4",
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
              "id": "3fcc9d4e-6200-49c4-b2c6-1af81fc93d22"
            }
          ]
        },
        {
          "id": "1ab2e3e6-2a11-49aa-9650-79c55e5d2033",
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
              "id": "10d2cc50-808f-4668-8016-54a767231ca5"
            }
          ]
        },
        {
          "id": "a1591e1b-5b04-4b79-831c-c21a9e3c6fd1",
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
              "id": "33878e71-0bfe-43b3-a86b-e3154b6cb147"
            }
          ]
        },
        {
          "id": "76af69e6-de4a-4318-94a5-c92ba0fca67f",
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
              "id": "5705b1fa-5bbc-451c-8cd9-a4e11bbc58ff"
            }
          ]
        },
        {
          "id": "d1161626-3feb-4b6e-9f1e-cee7cd6a0e99",
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
              "id": "64bc6cc3-9c2b-442f-98e0-efd1f600341e"
            }
          ]
        },
        {
          "id": "09565458-31da-4ca0-a6f5-fc750dfff408",
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
              "id": "869f4211-232f-40fc-a192-a23d1c6c6b93"
            }
          ]
        },
        {
          "id": "7f481244-feeb-44d2-9187-6cde4fa748ce",
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
              "id": "01456dc5-01be-486d-9da6-e5bf980e5c5e"
            }
          ]
        },
        {
          "id": "2409b56b-d933-40dd-9974-a75e772ccdfc",
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
              "id": "231743f4-c51f-47a6-b8af-384041ece40f"
            }
          ]
        },
        {
          "id": "b05a8d20-6056-45b8-8e4d-7309409e4657",
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
              "id": "d62c21bb-1406-4403-bd51-48afc2be4c8b"
            }
          ]
        },
        {
          "id": "34430c1b-9f55-4315-a9c8-f5c2ac7f81e5",
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
              "id": "cd8913e4-151e-4f1f-84cc-b2cc9004b54d"
            }
          ]
        },
        {
          "id": "f5e05fd6-7918-429b-9711-98e4b57c53c0",
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
              "id": "9b21f0c2-baf4-4dec-8b18-c69317ea659d"
            }
          ]
        },
        {
          "id": "a790f7bc-e86c-4a17-a695-bbabc75663c2",
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
              "id": "a65d5b56-49b0-4cb4-8d7e-4b6d77d7ce9e"
            }
          ]
        },
        {
          "id": "40c51e66-4be6-4269-aef5-d84f479a3d5e",
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
              "id": "489c345e-88f3-46f2-a6b3-c3b099c4d148"
            }
          ]
        },
        {
          "id": "cfe74272-3205-4abc-8042-30f51cd7b509",
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
              "id": "38b552d0-5396-4259-98b6-0a6020af176f"
            }
          ]
        },
        {
          "id": "3167a07a-7910-4252-b31e-fd63336d00b4",
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
              "id": "c39fa654-d6d2-4f57-8419-751950212270"
            }
          ]
        },
        {
          "id": "dd55e5ce-eb2e-4028-96bc-f4e1fcc87148",
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
              "id": "5d2b2576-0310-452b-961c-edf51ccf4e27"
            }
          ]
        },
        {
          "id": "291e8a77-38ca-4285-9ce5-2a8f9dd5325b",
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
              "id": "d33c7020-9124-4ad5-9ae8-481f29f54270"
            }
          ]
        },
        {
          "id": "9c9d501b-88e7-4799-9d40-f3c48f004d52",
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
              "id": "dbcfcfa5-777c-47af-90fc-939be9d18ca4"
            }
          ]
        },
        {
          "id": "3a8db786-a928-45ab-a2ea-76cb0a534886",
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
              "id": "96b55b92-744a-478a-87dd-d96e773e0e89"
            }
          ]
        },
        {
          "id": "7cf19ffc-a74c-4b36-b35e-a1952d9cd184",
          "name": "v2.imports.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/imports/:id.json"
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
            "description": "Fetches an import, by ID only.\n\nAdmin users can access imports for the entire team, but non-admin users can only access their own imports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b84d172-e3e8-4159-9f30-f29da4a06bb9"
            }
          ]
        },
        {
          "id": "4bb8a9d8-d247-4f15-b155-d519993e69c7",
          "name": "v2.imports.id.json.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/imports/:id.json"
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
            "description": "Updates an import, by ID only.\n\nAdmin users can access imports for the entire team, but non-admin users can only access their own imports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25baff68-972b-4b8f-9f70-cf7f38818b87"
            }
          ]
        },
        {
          "id": "503df60d-0692-4542-a855-b87ed3487ad3",
          "name": "v2.imports.id.json.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/imports/:id.json"
              ],
              "query": [
                {
                  "key": "undo",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Deletes an import, by ID only. The associated people can be deleted as part of the deletion process.\n\nAdmin users can access imports for the entire team, but non-admin users can only access their own imports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f3f5fde-5305-45f9-b34f-1a80b63b4fef"
            }
          ]
        },
        {
          "id": "92e5878c-a01a-44d5-9e7a-9a4631bcf725",
          "name": "v2.me.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/me.json",
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
            "description": "Authenticated user information. This endpoint does not accept any parameters as it is\nrepresents your authenticated user. The \"Users\" resource provides user information\nfor other users on the team."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d7aca50-454e-4494-b128-d1e07ad0d8e7"
            }
          ]
        },
        {
          "id": "ff33abf7-804a-4f42-b1f9-85db6263a66a",
          "name": "v2.notes.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/notes.json?associated_with_id=%7B%7D&associated_with_type=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple note records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b769d469-f5c8-4bf4-8d21-713f9a91c95c"
            }
          ]
        },
        {
          "id": "99ae1f1f-c4be-47cc-8a57-318a9f0a1544",
          "name": "v2.notes.json.post",
          "request": {
            "url": "http://api.salesloft.com/v2/notes.json",
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
                  "key": "associated_with_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the item with which the note is associated"
                },
                {
                  "key": "associated_with_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Case insensitive type of item with which the note is associated"
                },
                {
                  "key": "call_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the call with which the note is associated"
                },
                {
                  "key": "content",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of the note"
                },
                {
                  "key": "skip_crm_sync",
                  "value": "{}",
                  "disabled": false,
                  "description": "Boolean indicating if the CRM sync should be skipped"
                }
              ]
            },
            "description": "Creates a note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2790f12f-dd0e-441b-aac7-0caada6ab310"
            }
          ]
        },
        {
          "id": "1ac89461-015d-4922-9464-a62fb52b13b6",
          "name": "v2.notes.id.json.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/notes/:id.json"
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
            "description": "Fetches a note, by ID only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fd11b0a-ec1e-4d6d-b467-2ea78d7f308f"
            }
          ]
        },
        {
          "id": "b87a2350-2b49-4ea2-92c5-1254822545dd",
          "name": "v2.notes.id.json.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.salesloft.com",
              "path": [
                "v2/notes/:id.json"
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
                  "key": "call_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the call with which the note is associated"
                },
                {
                  "key": "content",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of the note"
                }
              ]
            },
            "description": "Updates a note. Any changes to the note or associated records will not reflect in Salesforce.com."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cd3f99f-1989-41bb-ad82-382c529fef37"
            }
          ]
        },
        {
          "id": "917c691a-9e40-4e91-b609-79130eacf6dd",
          "name": "v2.people.json.get",
          "request": {
            "url": "http://api.salesloft.com/v2/people.json?email_addresses=%7B%7D&ids=%7B%7D&include_paging_counts=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&updated_at=%7B%7D",
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
            "description": "Fetches multiple person records. The records can be filtered, paged, and sorted according to\nthe respective parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b35cf0b-88f1-4c03-a7af-ff2d20f3e5eb"
            }
          ]
        },
        {
          "id": "066f123a-9cd0-409c-8e2c-32cc676c687a",
          "name": "v2.people.json.post",
          "request": {
            "url": "http://api.salesloft.com/v2/people.json",
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
                  "key": "account_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the Account to link this person to"
                },
                {
                  "key": "autotag_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "Whether the date should be added to this person as a tag"
                },
                {
                  "key": "city",
                  "value": "{}",
                  "disabled": false,
                  "description": "City"
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
                  "key": "do_not_contact",
                  "value": "{}",
                  "disabled": false,
                  "description": "Whether this person can not be contacted"
                },
                {
                  "key": "email_address",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address"
                },
                {
                  "key": "first_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "First name"
                },
                {
                  "key": "home_phone",
                  "value": "{}",
                  "disabled": false,
                  "description": "Home phone without formatting"
                },
                {
                  "key": "import_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the Import this person is a part of"
                },
                {
                  "key": "last_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Last name"
                },
                {
                  "key": "linkedin_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Linkedin URL"
                },
                {
                  "key": "locale",
                  "value": "{}",
                  "disabled": false,
                  "description": "Time locale of the person"
                },
                {
                  "key": "mobile_phone",
                  "value": "{}",
                  "disabled": false,
                  "description": "Mobile phone without formatting"
                },
                {
                  "key": "owner_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the User that owns this person"
                },
                {
                  "key": "personal_email_address",
                  "value": "{}",
                  "disabled": false,
                  "description": "Personal email address"
                },
                {
                  "key": "personal_website",
                  "value": "{}",
                  "disabled": false,
                  "description": "The website of this person"
                },
                {
                  "key": "person_company_industry",
                  "value": "{}",
                  "disabled": false,
                  "description": "Company industry"
                },
                {
                  "key": "person_company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Company name"
                },
                {
                  "key": "person_company_website",
                  "value": "{}",
                  "disabled": false,
                  "description": "Company website"
                },
                {
                  "key": "person_stage_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the PersonStage of this person"
                },
                {
                  "key": "phone",
                  "value": "{}",
                  "disabled": false,
                  "description": "Phone without formatting"
                },
                {
                  "key": "phone_extension",
                  "value": "{}",
                  "disabled": false,
                  "description": "Phone extension without formatting"
                },
                {
                  "key": "secondary_email_address",
                  "value": "{}",
                  "disabled": false,
                  "description": "Alternate email address"
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": "State"
                },
                {
                  "key": "tags",
                  "value": "{}",
                  "disabled": false,
                  "description": "All tags applied to this person"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "Job title"
                },
                {
                  "key": "twitter_handle",
                  "value": "{}",
                  "disabled": false,
                  "description": "The twitter handle of this person"
                },
   