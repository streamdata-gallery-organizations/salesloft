---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Create an account
  description: |-
    Creates an account.

    "domain" must be unique on the current team.
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