---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch an email
  description: Fetches an email, by ID only.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/accounts.json:
    get:
      summary: List accounts
      description: |-
        Fetches multiple account records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.accounts.json.get
      x-api-path-slug: v2accounts-json-get
      parameters:
      - in: query
        name: domain
        description: Domain of the accounts to fetch
      - in: query
        name: ids
        description: IDs of accounts to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_contacted_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Accounts
    post:
      summary: Create an account
      description: |-
        Creates an account.

        "domain" must be unique on the current team.
      operationId: v2.accounts.json.post
      x-api-path-slug: v2accounts-json-post
      parameters:
      - in: formData
        name: city
        description: City
      - in: formData
        name: company_stage_id
        description: ID of the CompanyStage assigned to this Account
      - in: formData
        name: company_type
        description: Type of the Accounts company
      - in: formData
        name: conversational_name
        description: Conversational name of the Account
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: description
        description: Description
      - in: formData
        name: domain
        description: Website domain, not a fully qualified URI
      - in: formData
        name: do_not_contact
        description: Whether this company can not be contacted
      - in: formData
        name: founded
        description: Date or year of founding
      - in: formData
        name: industry
        description: Industry
      - in: formData
        name: linkedin_url
        description: Full LinkedIn url
      - in: formData
        name: locale
        description: Time locale
      - in: formData
        name: name
        description: Account Full Name
      - in: formData
        name: owner_id
        description: ID of the User that owns this Account
      - in: formData
        name: phone
        description: Phone number without formatting
      - in: formData
        name: postal_code
        description: Postal code
      - in: formData
        name: revenue_range
        description: Estimated revenue range
      - in: formData
        name: size
        description: Estimated number of people in employment
      - in: formData
        name: state
        description: State
      - in: formData
        name: street
        description: Street name and number
      - in: formData
        name: tags
        description: All tags applied to this Account
      - in: formData
        name: twitter_handle
        description: Twitter handle, with @
      - in: formData
        name: website
        description: Website
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Account
  /v2/accounts/{id}.json:
    delete:
      summary: Delete an account
      description: |-
        Deletes an account. This operation is not reversible without contacting support.
        This operation can be called multiple times successfully.

        Deleting an account will remove all connected people from that account.
      operationId: v2.accounts.id.json.delete
      x-api-path-slug: v2accountsid-json-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Account
    get:
      summary: Fetch an account
      description: Fetches an account, by ID only.
      operationId: v2.accounts.id.json.get
      x-api-path-slug: v2accountsid-json-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Account
    put:
      summary: Update an existing Account
      description: |-
        Updates an account.

        "domain" must be unique on the current team.
      operationId: v2.accounts.id.json.put
      x-api-path-slug: v2accountsid-json-put
      parameters:
      - in: formData
        name: city
        description: City
      - in: formData
        name: company_stage_id
        description: ID of the CompanyStage assigned to this Account
      - in: formData
        name: company_type
        description: Type of the Accounts company
      - in: formData
        name: conversational_name
        description: Conversational name of the Account
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: description
        description: Description
      - in: formData
        name: domain
        description: Website domain, not a fully qualified URI
      - in: formData
        name: do_not_contact
        description: Whether this company can not be contacted
      - in: formData
        name: founded
        description: Date or year of founding
      - in: path
        name: id
        description: Account ID
      - in: formData
        name: industry
        description: Industry
      - in: formData
        name: linkedin_url
        description: Full LinkedIn url
      - in: formData
        name: locale
        description: Time locale
      - in: formData
        name: name
        description: Account Full Name
      - in: formData
        name: owner_id
        description: ID of the User that owns this Account
      - in: formData
        name: phone
        description: Phone number without formatting
      - in: formData
        name: postal_code
        description: Postal code
      - in: formData
        name: revenue_range
        description: Estimated revenue range
      - in: formData
        name: size
        description: Estimated number of people in employment
      - in: formData
        name: state
        description: State
      - in: formData
        name: street
        description: Street name and number
      - in: formData
        name: tags
        description: All tags applied to this Account
      - in: formData
        name: twitter_handle
        description: Twitter handle, with @
      - in: formData
        name: website
        description: Website
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Existing
      - Account
  /v2/action_details/call_instructions.json:
    get:
      summary: List call instructions
      description: |-
        Fetches multiple call instruction records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.action_details.call_instructions.json.get
      x-api-path-slug: v2action-detailscall-instructions-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of call instructions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Call
      - Instructions
  /v2/action_details/call_instructions/{id}.json:
    get:
      summary: Fetch a call instructions
      description: Fetches a call instruction, by ID only.
      operationId: v2.action_details.call_instructions.id.json.get
      x-api-path-slug: v2action-detailscall-instructionsid-json-get
      parameters:
      - in: path
        name: id
        description: Call instructions ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
      - Instructions
  /v2/actions.json:
    get:
      summary: List actions
      description: |-
        Fetches multiple action records. The records can be filtered, paged, and sorted according to
        the respective parameters. Only actions that are currently "in_progess" will be returned by
        this endpoint.
      operationId: v2.actions.json.get
      x-api-path-slug: v2actions-json-get
      parameters:
      - in: query
        name: due_on
        description: Equality filters that are applied to the due_on field
      - in: query
        name: ids
        description: IDs of actions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: step_id
        description: Fetch actions by step ID
      - in: query
        name: type
        description: Filter actions by type
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Actions
  /v2/actions/{id}.json:
    get:
      summary: Fetch an action
      description: |-
        Fetches an action, by ID only.
        This endpoint will only return actions that are in_progress or pending_activity.
        Once an action is complete, the request for that action will return a 404 status code.
      operationId: v2.actions.id.json.get
      x-api-path-slug: v2actionsid-json-get
      parameters:
      - in: path
        name: id
        description: Action ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Action
  /v2/activities/calls.json:
    get:
      summary: List calls
      description: |-
        Fetches multiple call records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.calls.json.get
      x-api-path-slug: v2activitiescalls-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of calls to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Calls
  /v2/activities/calls/{id}.json:
    get:
      summary: Fetch a call
      description: Fetches a call, by ID only.
      operationId: v2.activities.calls.id.json.get
      x-api-path-slug: v2activitiescallsid-json-get
      parameters:
      - in: path
        name: id
        description: Call ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
  /v2/activities/emails.json:
    get:
      summary: List emails
      description: |-
        Fetches multiple email records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.emails.json.get
      x-api-path-slug: v2activitiesemails-json-get
      parameters:
      - in: query
        name: bounced
        description: Filters emails by whether they have bounced or not
      - in: query
        name: ids
        description: IDs of emails to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Emails
  /v2/activities/emails/{id}.json:
    get:
      summary: Fetch an email
      description: Fetches an email, by ID only.
      operationId: v2.activities.emails.id.json.get
      x-api-path-slug: v2activitiesemailsid-json-get
      parameters:
      - in: path
        name: id
        description: Email ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---