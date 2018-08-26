{
  "info": {
    "name": "SalesLoft Fetch a step",
    "_postman_id": "807c195e-5fa5-4da8-a88b-25514fc0121e",
    "description": "Fetches a step, by ID only.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sales",
      "item": [
        {
          "id": "62b21f48-091a-4199-b401-418bb2cff614",
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
              "id": "a0744c12-8901-4a0e-8071-ed734a3931ab"
            }
          ]
        },
        {
          "id": "de27c72c-b50c-4d26-a6b9-08c52beea295",
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
              "id": "f3140f32-b7c9-499c-a183-15a78521e686"
            }
          ]
        },
        {
          "id": "fd136eb8-3c46-4893-b4f2-174da3ba83dc",
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
              "id": "532f87ab-c80b-463c-8046-bff629538bd3"
            }
          ]
        },
        {
          "id": "7efe0a44-05b5-409b-a338-8f5000d668c4",
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
              "id": "c1974b6b-9151-4081-a5ba-a3f58c50b471"
            }
          ]
        },
        {
          "id": "a514e760-35bd-4bc1-b409-2c0d10be4162",
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
              "id": "d7462459-2c04-4c88-9e2b-00afe187d94d"
            }
          ]
        },
        {
          "id": "1829bf7f-e366-4ac1-bf56-c2c0231cc0e9",
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
              "id": "56caae1c-8488-42c9-bbea-f104c572a56f"
            }
          ]
        },
        {
          "id": "e56eb555-957d-4488-a1a8-6848a75f6e58",
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
              "id": "c6b83929-cf1a-45aa-8cfc-8a683b583b92"
            }
          ]
        },
        {
          "id": "5c968d81-f34a-4619-86c5-a2b88f6fb581",
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
              "id": "02e77642-4b06-483e-b6f9-82790af8e464"
            }
          ]
        },
        {
          "id": "3f8a5e21-94ac-4e64-bb37-40ef1c5d1e7a",
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
              "id": "5bd89324-4d3d-43cd-b4f0-fd3a94a3cced"
            }
          ]
        },
        {
          "id": "8c332c17-8798-4300-ac2c-34e2e6dd42fb",
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
              "id": "4ce78776-6a98-4155-b528-d932f8e17069"
            }
          ]
        },
        {
          "id": "13e3c3bf-9e0d-42a2-90ba-4b8f3bcbbc2d",
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
              "id": "b8d64fb3-cb5c-4de0-8e62-d361e595df68"
            }
          ]
        },
        {
          "id": "6d2d2869-b841-4cb4-97f9-d919b9fc0f61",
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
              "id": "74b705a8-6d51-4fc9-a01b-5652d30bb79e"
            }
          ]
        },
        {
          "id": "e7a1e70c-8f6b-4985-a328-7b1df9fcf1b5",
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
              "id": "995e727c-6ac1-4186-aaf2-b4686558c1bf"
            }
          ]
        },
        {
          "id": "7e40ec15-9dc8-4dea-9f73-5e57a6c2d17f",
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
              "id": "a158cbb5-e9e0-4c5c-b273-27ec1cf99e59"
            }
          ]
        },
        {
          "id": "c073ddee-3117-4b52-8275-66eb51b2bb8a",
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
              "id": "1d1f5dcd-66da-43c3-b026-18f94779580f"
            }
          ]
        },
        {
          "id": "4a38dcf7-c64c-470c-bdf6-d057300016db",
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
              "id": "7b38a103-a716-4c08-94a6-96da2b7de6a4"
            }
          ]
        },
        {
          "id": "6e4ad66a-abc1-4000-9919-111e8df3884b",
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
              "id": "039c2a50-5505-4f9f-ab69-f2907d0ec7c1"
            }
          ]
        },
        {
          "id": "6a7df1fb-34eb-41c9-8e56-c8dd88deb26b",
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
              "id": "a645fa34-e2f8-4f8c-bec1-86b86e16181e"
            }
          ]
        },
        {
          "id": "eeeb714a-8b00-4967-9471-c91a539e4b1f",
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
              "id": "3273528f-9551-4e9b-a507-659e65f395bb"
            }
          ]
        },
        {
          "id": "004e3893-e74a-466e-8153-f32cfe5bcf0b",
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
              "id": "96093cea-5cd0-4948-9acb-48a8b988f0d6"
            }
          ]
        },
        {
          "id": "dbd3c901-5376-4d09-a3d8-75de29e7557d",
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
              "id": "cd2106d4-60c4-43e9-adc9-9d6d3f40ca47"
            }
          ]
        },
        {
          "id": "b6f297a1-247c-41bd-9e5e-118407a67703",
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
              "id": "92d1f7de-1388-4d88-a53a-a8b87f96e0ff"
            }
          ]
        },
        {
          "id": "90b3b040-c482-436a-bb13-97a24688ce4f",
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
              "id": "1703bf9f-0f2e-4509-ba6c-86610d345da0"
            }
          ]
        },
        {
          "id": "b28d3ffe-4db7-49a9-8e24-423443fb30af",
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
              "id": "5c2659c4-39b1-41e9-acd8-41da88cc1c51"
            }
          ]
        },
        {
          "id": "439f9f3b-fc6b-4418-b827-12d0a496d40a",
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
              "id": "8595ce23-1396-4d09-a97b-5a711c012495"
            }
          ]
        },
        {
          "id": "951c0643-9f27-4350-9765-04abd7628175",
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
              "id": "5c12b38f-04ee-481d-918f-04c81a7f2cdb"
            }
          ]
        },
        {
          "id": "78459b1a-a2f2-4ae4-9675-a4c4461a7eef",
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
              "id": "10f3b837-a121-4762-8e28-5229d8811eb9"
            }
          ]
        },
        {
          "id": "41a3226e-f2bf-444f-bef2-82a0101a6dc8",
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
              "id": "860aec62-dee5-4781-a561-c5b89efe19fb"
            }
          ]
        },
        {
          "id": "cf22f017-6a45-4be8-8cbf-6c33f1f7e88c",
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
              "id": "88636440-bd30-4a30-9002-75da6d94613c"
            }
          ]
        },
        {
          "id": "82549ec6-2d52-4b31-bdc9-904ceb5b1ad0",
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
              "id": "09f7341a-68e2-4d69-89e9-0e23473ecd82"
            }
          ]
        },
        {
          "id": "20b3d014-afdf-46be-a806-16793410950b",
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
              "id": "9f923dd5-0f40-4f2c-b0e5-31caded32725"
            }
          ]
        },
        {
          "id": "f49740c4-7d80-446d-9505-9154f2594980",
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
              "id": "05629c05-b109-4c1f-9f04-df12108d4421"
            }
          ]
        },
        {
          "id": "f0aadd0a-7453-41f7-9840-dc1f683cbff0",
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
              "id": "09c648ea-0864-4638-8359-326b6c548773"
            }
          ]
        },
        {
          "id": "84a0abf3-02f1-4232-b628-131c795eb057",
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
              "id": "ffa31788-f417-4f14-8f68-1477ac90491f"
            }
          ]
        },
        {
          "id": "21bc6a04-679f-4092-838b-09652ad98229",
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
              "id": "e1c96fb9-5bc0-4fc4-a7ce-a92aa9f57152"
            }
          ]
        },
        {
          "id": "c6b70088-d0c9-4f57-9fbe-2f8e4d835600",
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
              "id": "d2c18f41-db11-4424-942b-0053027836b0"
            }
          ]
        },
        {
          "id": "26f42ad4-8ae2-4960-9953-1a836728d0fb",
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
              "id": "1ee08361-5781-4455-ad81-3548c35c0d16"
            }
          ]
        },
        {
          "id": "7c6ffc5a-7512-4c84-9225-498cbb4a931d",
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
              "id": "bdfc3d9a-c0b5-41a8-8586-cc48c446096c"
            }
          ]
        },
        {
          "id": "24434581-7d3f-4d12-91d0-f2e0a713adc1",
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
              "id": "7feeabd4-5f60-4206-9d2a-ca7bd1c866e2"
            }
          ]
        },
        {
          "id": "c399b580-5822-4e19-806c-bce27366fbdd",
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
              "id": "a9504a7e-a515-4f07-8c62-21b46487fa09"
            }
          ]
        },
        {
          "id": "81d3a0ba-2e94-43a1-b202-e3699c504181",
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
              "id": "54b7911a-2016-49b6-9cfa-8bbea564c2d2"
            }
          ]
        },
        {
          "id": "4a3efd6f-e20f-403c-8404-af20e720cc66",
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
        