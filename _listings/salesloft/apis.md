---
name: SalesLoft
x-slug: salesloft
description: SalesLoft, the leading sales engagement platform, transforms the way
  sellers engage with their customers by delivering a better selling experience. Our
  sales engagement platform helps teams set and execute on a cadence of phone, email,
  and social communications to convert more target accounts into customer accounts.
  The platform equips sales leaders with new capabilities to test, learn and adapt
  to ensure their sales reps execute on the most effective selling process for their
  account-based approach. SalesLoft delivers access to an extensive ecosystem of 3rd
  party integrations allowing teams to perform all their sales engagement from a single
  platform.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
x-kinRank: "7"
x-alexaRank: "0"
tags: SalesLoft
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/apis.md
specificationVersion: "0.14"
apis:
- name: SalesLoft - List accounts
  x-api-slug: v2accounts-json-get
  description: |-
    Fetches multiple account records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accounts-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accounts-json-get-openapi.md
- name: SalesLoft - Create an account
  x-api-slug: v2accounts-json-post
  description: |-
    Creates an account.

    "domain" must be unique on the current team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accounts-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accounts-json-post-openapi.md
- name: SalesLoft - Delete an account
  x-api-slug: v2accountsid-json-delete
  description: |-
    Deletes an account. This operation is not reversible without contacting support.
    This operation can be called multiple times successfully.

    Deleting an account will remove all connected people from that account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accountsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accountsid-json-delete-openapi.md
- name: SalesLoft - Fetch an account
  x-api-slug: v2accountsid-json-get
  description: Fetches an account, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accountsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accountsid-json-get-openapi.md
- name: SalesLoft - Update an existing Account
  x-api-slug: v2accountsid-json-put
  description: |-
    Updates an account.

    "domain" must be unique on the current team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accountsid-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2accountsid-json-put-openapi.md
- name: SalesLoft - List call instructions
  x-api-slug: v2action-detailscall-instructions-json-get
  description: |-
    Fetches multiple call instruction records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2action-detailscall-instructions-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2action-detailscall-instructions-json-get-openapi.md
- name: SalesLoft - Fetch a call instructions
  x-api-slug: v2action-detailscall-instructionsid-json-get
  description: Fetches a call instruction, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2action-detailscall-instructionsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2action-detailscall-instructionsid-json-get-openapi.md
- name: SalesLoft - List actions
  x-api-slug: v2actions-json-get
  description: |-
    Fetches multiple action records. The records can be filtered, paged, and sorted according to
    the respective parameters. Only actions that are currently "in_progess" will be returned by
    this endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2actions-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2actions-json-get-openapi.md
- name: SalesLoft - Fetch an action
  x-api-slug: v2actionsid-json-get
  description: |-
    Fetches an action, by ID only.
    This endpoint will only return actions that are in_progress or pending_activity.
    Once an action is complete, the request for that action will return a 404 status code.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2actionsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2actionsid-json-get-openapi.md
- name: SalesLoft - List calls
  x-api-slug: v2activitiescalls-json-get
  description: |-
    Fetches multiple call records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiescalls-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiescalls-json-get-openapi.md
- name: SalesLoft - Fetch a call
  x-api-slug: v2activitiescallsid-json-get
  description: Fetches a call, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiescallsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiescallsid-json-get-openapi.md
- name: SalesLoft - List emails
  x-api-slug: v2activitiesemails-json-get
  description: |-
    Fetches multiple email records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiesemails-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiesemails-json-get-openapi.md
- name: SalesLoft - Fetch an email
  x-api-slug: v2activitiesemailsid-json-get
  description: Fetches an email, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiesemailsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2activitiesemailsid-json-get-openapi.md
- name: SalesLoft - List cadence memberships
  x-api-slug: v2cadence-memberships-json-get
  description: |-
    Fetches multiple cadence membership records. The records can be filtered, paged, and sorted according to
    the respective parameters. A cadence membership is the association between a person and their current and
    historical time on a cadence. Cadence membership records are mutable and change over time. If a person is
    added to a cadence and re-added to the same cadence in the future, there is a single membership record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-memberships-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-memberships-json-get-openapi.md
- name: SalesLoft - Create a cadence membership
  x-api-slug: v2cadence-memberships-json-post
  description: |-
    Adds a person to a cadence. person_id and cadence_id are required, and must be visible to the authenticated user. user_id will
    default to the authenticated user, but can be set to any visible user on the authenticated team.

    A person cannot be added to a cadence on behalf of a teammate unless the cadence is a team cadence, or the cadence is owned by
    the teammate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-memberships-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-memberships-json-post-openapi.md
- name: SalesLoft - Delete a cadence membership
  x-api-slug: v2cadence-membershipsid-json-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-membershipsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-membershipsid-json-delete-openapi.md
- name: SalesLoft - Fetch a cadence membership
  x-api-slug: v2cadence-membershipsid-json-get
  description: Fetches a cadence membership, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-membershipsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadence-membershipsid-json-get-openapi.md
- name: SalesLoft - List cadences
  x-api-slug: v2cadences-json-get
  description: |-
    Fetches multiple cadence records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadences-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadences-json-get-openapi.md
- name: SalesLoft - Fetch a cadence
  x-api-slug: v2cadencesid-json-get
  description: Fetches a cadence, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadencesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2cadencesid-json-get-openapi.md
- name: SalesLoft - List call data records
  x-api-slug: v2call-data-records-json-get
  description: |-
    Fetches multiple call data records. The records can be filtered, paged, and sorted according to
    the respective parameters.

    Call data records are records of all inbound and outbound calls through SalesLoft. A call data record may
    be associated with a call, but does not have to be.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2call-data-records-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2call-data-records-json-get-openapi.md
- name: SalesLoft - Fetch a call data record
  x-api-slug: v2call-data-recordsid-json-get
  description: Fetches a call data record, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2call-data-recordsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2call-data-recordsid-json-get-openapi.md
- name: SalesLoft - List crm activities
  x-api-slug: v2crm-activities-json-get
  description: |-
    Fetches multiple crm activity records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2crm-activities-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2crm-activities-json-get-openapi.md
- name: SalesLoft - Fetch a crm activity
  x-api-slug: v2crm-activitiesid-json-get
  description: Fetches a crm activity, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2crm-activitiesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2crm-activitiesid-json-get-openapi.md
- name: SalesLoft - List custom fields
  x-api-slug: v2custom-fields-json-get
  description: |-
    Fetches multiple custom field records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fields-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fields-json-get-openapi.md
- name: SalesLoft - Create a custom field
  x-api-slug: v2custom-fields-json-post
  description: Creates a custom field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fields-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fields-json-post-openapi.md
- name: SalesLoft - Delete a custom field
  x-api-slug: v2custom-fieldsid-json-delete
  description: Deletes a custom field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fieldsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fieldsid-json-delete-openapi.md
- name: SalesLoft - Fetch a custom field
  x-api-slug: v2custom-fieldsid-json-get
  description: Fetches a custom field, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fieldsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fieldsid-json-get-openapi.md
- name: SalesLoft - Update a custom field
  x-api-slug: v2custom-fieldsid-json-put
  description: Update a custom field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fieldsid-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2custom-fieldsid-json-put-openapi.md
- name: SalesLoft - List email templates
  x-api-slug: v2email-templates-json-get
  description: |-
    Fetches multiple email template records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2email-templates-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2email-templates-json-get-openapi.md
- name: SalesLoft - Fetch an email template
  x-api-slug: v2email-templatesid-json-get
  description: Fetches an email template, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2email-templatesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2email-templatesid-json-get-openapi.md
- name: SalesLoft - List imports
  x-api-slug: v2imports-json-get
  description: Fetches multiple imports.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2imports-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2imports-json-get-openapi.md
- name: SalesLoft - Create an import
  x-api-slug: v2imports-json-post
  description: Creates an import.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2imports-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2imports-json-post-openapi.md
- name: SalesLoft - Delete an import
  x-api-slug: v2importsid-json-delete
  description: |-
    Deletes an import, by ID only. The associated people can be deleted as part of the deletion process.

    Admin users can access imports for the entire team, but non-admin users can only access their own imports.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2importsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2importsid-json-delete-openapi.md
- name: SalesLoft - Fetch an import
  x-api-slug: v2importsid-json-get
  description: |-
    Fetches an import, by ID only.

    Admin users can access imports for the entire team, but non-admin users can only access their own imports.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2importsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2importsid-json-get-openapi.md
- name: SalesLoft - Update an import
  x-api-slug: v2importsid-json-put
  description: |-
    Updates an import, by ID only.

    Admin users can access imports for the entire team, but non-admin users can only access their own imports.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2importsid-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2importsid-json-put-openapi.md
- name: SalesLoft - Fetch current user
  x-api-slug: v2me-json-get
  description: |-
    Authenticated user information. This endpoint does not accept any parameters as it is
    represents your authenticated user. The "Users" resource provides user information
    for other users on the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2me-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2me-json-get-openapi.md
- name: SalesLoft - List notes
  x-api-slug: v2notes-json-get
  description: |-
    Fetches multiple note records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notes-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notes-json-get-openapi.md
- name: SalesLoft - Create a note
  x-api-slug: v2notes-json-post
  description: Creates a note.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notes-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notes-json-post-openapi.md
- name: SalesLoft - Fetch a note
  x-api-slug: v2notesid-json-get
  description: Fetches a note, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notesid-json-get-openapi.md
- name: SalesLoft - Update a note
  x-api-slug: v2notesid-json-put
  description: Updates a note. Any changes to the note or associated records will
    not reflect in Salesforce.com.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notesid-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2notesid-json-put-openapi.md
- name: SalesLoft - List people
  x-api-slug: v2people-json-get
  description: |-
    Fetches multiple person records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2people-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2people-json-get-openapi.md
- name: SalesLoft - Create a person
  x-api-slug: v2people-json-post
  description: |-
    Creates a person. Either email_address or phone/last_name must be provided as a unique lookup
    on the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2people-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2people-json-post-openapi.md
- name: SalesLoft - Delete a person
  x-api-slug: v2peopleid-json-delete
  description: |-
    Deletes a person. This operation is not reversible without contacting support.
    This operation can be called multiple times successfully.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2peopleid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2peopleid-json-delete-openapi.md
- name: SalesLoft - Fetch a person
  x-api-slug: v2peopleid-json-get
  description: Fetches a person, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2peopleid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2peopleid-json-get-openapi.md
- name: SalesLoft - Update a person
  x-api-slug: v2peopleid-json-put
  description: Updates a person.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2peopleid-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2peopleid-json-put-openapi.md
- name: SalesLoft - List person stages
  x-api-slug: v2person-stages-json-get
  description: |-
    Fetches multiple person stage records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stages-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stages-json-get-openapi.md
- name: SalesLoft - Create a person stage
  x-api-slug: v2person-stages-json-post
  description: Creates a person stage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stages-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stages-json-post-openapi.md
- name: SalesLoft - Delete an person stage
  x-api-slug: v2person-stagesid-json-delete
  description: |-
    Deletes a person stage. This operation is not reversible without contacting support.
    This operation can be called multiple times successfully.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stagesid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stagesid-json-delete-openapi.md
- name: SalesLoft - Fetch a person stage
  x-api-slug: v2person-stagesid-json-get
  description: Fetches a person stage, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stagesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stagesid-json-get-openapi.md
- name: SalesLoft - Update a person stage
  x-api-slug: v2person-stagesid-json-put
  description: Updates a person stage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stagesid-json-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2person-stagesid-json-put-openapi.md
- name: SalesLoft - List caller ids
  x-api-slug: v2phone-numberscaller-ids-json-get
  description: |-
    Each entry is a possible caller ID match for the number. Multiple
    entries may be returned if the phone number is present on more than one
    person in the system.  Phone number should be in E.164 format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2phone-numberscaller-ids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2phone-numberscaller-ids-json-get-openapi.md
- name: SalesLoft - Fetch recording setting
  x-api-slug: v2phone-numbersrecording-settingsid-json-get
  description: |-
    Fetches the recording status for a given phone number, based on Do Not Record and Recording Governance for your team.
    Phone number should be in E.164 format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2phone-numbersrecording-settingsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2phone-numbersrecording-settingsid-json-get-openapi.md
- name: SalesLoft - List steps
  x-api-slug: v2steps-json-get
  description: |-
    Fetches multiple step records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2steps-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2steps-json-get-openapi.md
- name: SalesLoft - Fetch a step
  x-api-slug: v2stepsid-json-get
  description: Fetches a step, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2stepsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2stepsid-json-get-openapi.md
- name: SalesLoft - List successes
  x-api-slug: v2successes-json-get
  description: |-
    Fetches multiple success records. The records can be filtered, paged, and sorted according to
    the respective parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2successes-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2successes-json-get-openapi.md
- name: SalesLoft - Fetch current team
  x-api-slug: v2team-json-get
  description: Fetches the team of the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2team-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2team-json-get-openapi.md
- name: SalesLoft - List team templates
  x-api-slug: v2team-templates-json-get
  description: |-
    Fetches multiple team template records. The records can be filtered, paged, and sorted according to
    the respective parameters.

    Team templates are templates that are available team-wide. Admins may use
    team templates to create original content for the entire team, monitor version control to ensure templates are always up to date,
    and track template performance across the entire organization. All metrics on a team template reflect usage across the team; individual metrics can be found with the email_templates API endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2team-templates-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2team-templates-json-get-openapi.md
- name: SalesLoft - Fetch a team template
  x-api-slug: v2team-templatesid-json-get
  description: Fetches a team template, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2team-templatesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2team-templatesid-json-get-openapi.md
- name: SalesLoft - List users
  x-api-slug: v2users-json-get
  description: |-
    Non Admin: Lists only your user, or all on team depending on group visibility policy
    Team Admin: Lists users associated with your team
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2users-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2users-json-get-openapi.md
- name: SalesLoft - Fetch a user
  x-api-slug: v2usersid-json-get
  description: Fetches a user, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2usersid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/salesloft/master/_listings/salesloft/v2usersid-json-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://salesforce.api.gallery.streamdata.io
- type: x-api-stack
  url: http://salesloft.stack.network
- type: x-blog
  url: https://salesloft.com/resources/blog/
- type: x-blog-rss
  url: https://salesloft.com/feed/
- type: x-developer
  url: https://developers.salesloft.com/api.html
- type: x-documentation
  url: https://developers.salesloft.com/api.html#!/Topic/Introduction
- type: x-github
  url: https://github.com/SalesLoft
- type: x-pricing
  url: https://salesloft.com/plans/
- type: x-support
  url: https://salesloft.com/support/
- type: x-twitter
  url: https://twitter.com/SalesLoft
- type: x-website
  url: http://salesloft.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---