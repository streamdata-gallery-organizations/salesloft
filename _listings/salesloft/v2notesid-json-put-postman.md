{
  "info": {
    "name": "SalesLoft Update a note",
    "_postman_id": "267b2c93-9697-4e80-867a-3d52fcfe0e7b",
    "description": "Updates a note. Any changes to the note or associated records will not reflect in Salesforce.com.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sales",
      "item": [
        {
          "id": "e4a5310d-8beb-45c7-99d8-1a85625cbed9",
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
              "id": "6d6224e4-96ba-4827-8e8d-719321496b4f"
            }
          ]
        },
        {
          "id": "08d2d219-fd40-4a2a-9118-d3b2a2c5a247",
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
              "id": "6004853d-e3f6-4a43-b4ec-38e0217f266d"
            }
          ]
        },
        {
          "id": "42734b4d-8fce-4fc7-8e6a-2c030088746c",
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
              "id": "266fb3a9-49f7-4d8e-9c64-ccbe3920f0be"
            }
          ]
        },
        {
          "id": "fe3ca8bf-46a5-4ddc-81f6-f123a280c2fb",
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
              "id": "f836f2f8-c012-457b-a505-3808081d5bc5"
            }
          ]
        },
        {
          "id": "989063c6-4831-4621-b02e-76b3a27a41c7",
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
              "id": "20d6d69f-5ff0-4a40-9756-ad2c224dda75"
            }
          ]
        },
        {
          "id": "f1f7f837-0e80-42c8-bed6-1a243e491672",
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
              "id": "b8e85f57-d9a0-48c6-898d-a53b6780df7e"
            }
          ]
        },
        {
          "id": "6633fca0-c44f-4751-a04d-5beb5b0835b3",
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
              "id": "bbfb782c-6d39-4ce8-8a4c-31d7c4545c10"
            }
          ]
        },
        {
          "id": "35bab6f2-45d0-4ff1-baf3-705580cb245f",
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
              "id": "5218d44f-a71c-462c-bb10-ad2b35510d6d"
            }
          ]
        },
        {
          "id": "be19203f-9914-4ed6-aa17-25234a6659dc",
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
              "id": "ee271872-9df8-496d-a00a-7d6735ce426e"
            }
          ]
        },
        {
          "id": "0db1ac99-cc20-442f-896a-af35ddcc114e",
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
              "id": "e574f6f1-9da1-4aea-a402-e70586b96fad"
            }
          ]
        },
        {
          "id": "9b89badc-1f15-4dad-bfdd-dfd1f83f10fa",
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
              "id": "356a782c-0ecd-4f39-9d0c-17fc09e8c5b3"
            }
          ]
        },
        {
          "id": "75fc158a-b653-4a50-ad72-23423e313dbb",
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
              "id": "6eb4b2fc-6cca-4efb-8a2d-2e28852b8385"
            }
          ]
        },
        {
          "id": "53e7d5e7-872a-408c-9024-d36e14d81f5e",
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
              "id": "d13e534b-8dee-4e21-9943-3c3c84a828e2"
            }
          ]
        },
        {
          "id": "b788b280-73ee-4f53-9a76-e59b44b9de58",
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
              "id": "4ded3b94-c12f-4c9e-8a96-abc1aa881885"
            }
          ]
        },
        {
          "id": "3a72fc4a-51e7-4304-aee0-4ebc9dd936ad",
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
              "id": "74ad07a4-2474-4ff0-90fb-bdf28b599784"
            }
          ]
        },
        {
          "id": "672ef865-355d-4b1b-a548-aaa6a44da2dd",
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
              "id": "d7210dd1-6db4-4c12-b535-545a7d231655"
            }
          ]
        },
        {
          "id": "749607ee-35c6-41ea-999a-6ae9896f2c7d",
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
              "id": "4ace1e18-3dbc-4765-b4e3-12af5a9315ba"
            }
          ]
        },
        {
          "id": "cd4a6f6a-e03e-4728-be93-6238aae7f3f5",
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
              "id": "9439fd4b-a9c7-4d45-aec5-aac46afa2a0d"
            }
          ]
        },
        {
          "id": "2a298f19-2538-433e-9957-ed667c303c41",
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
              "id": "455dc8bb-fed7-4cb8-8643-98f0cde5b223"
            }
          ]
        },
        {
          "id": "a4aee6c9-302f-4ef6-b231-636269015135",
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
              "id": "f740b3c9-6001-4b8a-aa6e-ed8f634157fa"
            }
          ]
        },
        {
          "id": "0548ffc2-08d7-4a5a-a026-d01465819e42",
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
              "id": "58f882fb-70eb-462b-aa0a-df91dd973a11"
            }
          ]
        },
        {
          "id": "45ba7010-e297-4ce4-8bdf-a54995abb3d8",
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
              "id": "608cc167-3149-4de9-a2e3-57f221d9d804"
            }
          ]
        },
        {
          "id": "3a33ef90-0003-4f66-a796-bb1e6c7264fd",
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
              "id": "f515999a-0c70-445c-a1cb-16692e9ab630"
            }
          ]
        },
        {
          "id": "270cea99-648a-4ad3-9985-41f0e625cdd5",
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
              "id": "b09b1502-4c2c-492b-9700-3ea2b8f442c1"
            }
          ]
        },
        {
          "id": "6b14782b-f348-48ed-840c-8ba861edbf48",
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
              "id": "3c77d541-f1ee-48c5-a309-1546f1499d94"
            }
          ]
        },
        {
          "id": "9cdb2cc5-307f-4fca-b5ae-a71480f4b70f",
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
              "id": "d5af38c6-37a1-4a78-9c96-2759f0917e46"
            }
          ]
        },
        {
          "id": "41b58176-815e-4bac-bc18-34b679409ef2",
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
              "id": "10962dca-9651-4d57-9cf3-600ad5de838f"
            }
          ]
        },
        {
          "id": "6b9b3e5c-498a-4e64-8b8b-a4810912d7b3",
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
              "id": "a76eb3d6-1353-4de3-bb81-f694ef66443f"
            }
          ]
        },
        {
          "id": "57e4d651-8ae8-4939-b01c-bf9b62e7cd1a",
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
              "id": "d62c04ca-70d2-405d-9e90-58d926446740"
            }
          ]
        },
        {
          "id": "9677e233-2367-4fb0-bf26-83cbf439e7d1",
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
              "id": "043cc93e-cd03-4702-ba72-d3448cf578b8"
            }
          ]
        },
        {
          "id": "5cb816dd-71a7-485f-b5c1-ba7c33b7df41",
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
              "id": "709051bb-ae3e-47c2-b514-11e48a2a69b1"
            }
          ]
        },
        {
          "id": "8e1b9a3a-cd16-4ab6-8da9-1ac8518fe3e7",
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
              "id": "aea6ba08-73b3-4a7a-a01d-b5e22ffe10c5"
            }
          ]
        },
        {
          "id": "522bd14b-5b9b-4557-a768-63fbb5fb1bda",
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
              "id": "3262c636-a1fa-4fb1-be3f-6b7769d34502"
            }
          ]
        },
        {
          "id": "0c5708bd-c5f1-44bf-8c8d-1f699d3f4415",
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
              "id": "b8bb389a-0f7b-46ab-9c25-b85f44f35028"
            }
          ]
        },
        {
          "id": "31354c12-438b-4968-a572-41e3fd413d4d",
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
              "id": "44cbe602-76d5-4135-bfe3-b469f53197a0"
            }
          ]
        },
        {
          "id": "bf7cf07a-26d4-465d-bd5e-a81b19db9a68",
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
              "id": "2dbe1b28-3129-41af-9a3c-1114009748fb"
            }
          ]
        },
        {
          "id": "8f68c699-fe66-4fc3-bfbe-77f9e1112232",
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
              "id": "572192af-3864-4e77-9744-8673297e5be5"
            }
          ]
        },
        {
          "id": "7c0e4313-53e0-4900-a3a2-efda52c1591b",
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
              "id": "4bc45691-e44f-4743-ac59-4a77e6a2fa5b"
            }
          ]
        },
        {
          "id": "5f14953c-6503-4beb-9943-e7ba9bbe0e9c",
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
              "id": "a417b8ff-8c0f-4f6b-abee-9656d3a65f3f"
            }
          ]
        },
        {
          "id": "9d4fa950-24d5-46a6-b5e5-5342cc0b97e5",
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
              "id": "2b12a0a7-289d-413c-a9b6-de01af753f2d"
            }
          ]
        }
      ]
    }
  ]
}