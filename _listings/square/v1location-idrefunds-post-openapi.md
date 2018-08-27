---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Issues a refund for a previously processed payment. You
    must issue a refund within 60 days of the associated payment.
  description: Issues a refund for a previously processed payment. You must issue
    a refund within 60 days of the associated payment.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/me/timecards/{timecard_id}/events:
    get:
      summary: Provides summary information for all events associated with a particular
        timecard.
      description: Provides summary information for all events associated with a particular
        timecard.
      operationId: ListTimecardEvents
      x-api-path-slug: v1metimecardstimecard-idevents-get
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to list events for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Events
      - Associated
      - Particular
      - Timecard
  /v1/{location_id}/bank-accounts:
    get:
      summary: Provides non-confidential details for all of a location's associated
        bank accounts. This endpoint does not provide full bank account numbers, and
        there is no way to obtain a full bank account number with the Connect API.
      description: Provides non-confidential details for all of a location's associated
        bank accounts. This endpoint does not provide full bank account numbers, and
        there is no way to obtain a full bank account number with the Connect API.
      operationId: ListBankAccounts
      x-api-path-slug: v1location-idbankaccounts-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list bank accounts for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Non-confidential
      - Details
      - Of
      - Locations
      - Associated
      - Bank
      - Accounts
      - ""
      - This
      - Endpoint
      - Does
      - Not
      - Provide
      - Full
      - Bank
      - Account
      - Numbers
      - ""
      - There
      - Is
      - "No"
      - Way
      - To
      - Obtain
      - Full
      - Bank
      - Account
      - Number
      - Connect
  /v1/{location_id}/bank-accounts/{bank_account_id}:
    get:
      summary: Provides non-confidential details for a merchant's associated bank
        account. This endpoint does not provide full bank account numbers, and there
        is no way to obtain a full bank account number with the Connect API.
      description: Provides non-confidential details for a merchant's associated bank
        account. This endpoint does not provide full bank account numbers, and there
        is no way to obtain a full bank account number with the Connect API.
      operationId: RetrieveBankAccount
      x-api-path-slug: v1location-idbankaccountsbank-account-id-get
      parameters:
      - in: path
        name: bank_account_id
        description: The bank accounts Square-issued ID
      - in: path
        name: location_id
        description: The ID of the bank accounts associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Non-confidential
      - Detailsa
      - Merchants
      - Associated
      - Bank
      - Account
      - ""
      - This
      - Endpoint
      - Does
      - Not
      - Provide
      - Full
      - Bank
      - Account
      - Numbers
      - ""
      - There
      - Is
      - "No"
      - Way
      - To
      - Obtain
      - Full
      - Bank
      - Account
      - Number
      - Connect
  /v1/{location_id}/items/{item_id}:
    delete:
      summary: Deletes an existing item and all item variations associated with it.
      description: Deletes an existing item and all item variations associated with
        it.
      operationId: DeleteItem
      x-api-path-slug: v1location-iditemsitem-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - ""
      - Item
      - Variations
      - Associated
      - It
    get:
      summary: Provides the details for a single item, including associated modifier
        lists and fees.
      description: Provides the details for a single item, including associated modifier
        lists and fees.
      operationId: RetrieveItem
      x-api-path-slug: v1location-iditemsitem-id-get
      parameters:
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Item
      - ""
      - Including
      - Associated
      - Modifier
      - Lists
      - Fees
  /v1/{location_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Deletes an existing item modifier list and all modifier options associated
        with it.
      description: Deletes an existing item modifier list and all modifier options
        associated with it.
      operationId: DeleteModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - List
      - ""
      - Modifier
      - Options
      - Associated
      - It
  /v1/{location_id}/refunds:
    post:
      summary: Issues a refund for a previously processed payment. You must issue
        a refund within 60 days of the associated payment.
      description: Issues a refund for a previously processed payment. You must issue
        a refund within 60 days of the associated payment.
      operationId: v1.location_id.refunds.post
      x-api-path-slug: v1location-idrefunds-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the original payments associated location
      responses:
        200:
          description: OK
      tags:
      - Issues
      - Refunda
      - Previously
      - Processed
      - Payment
      - ""
      - You
      - Must
      - Issue
      - Refund
      - Within
      - "60"
      - Days
      - Of
      - Associated
      - Payment
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