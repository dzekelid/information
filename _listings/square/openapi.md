---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
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
  /v1/me:
    get:
      summary: Get a business's information.
      description: Get a business's information.
      operationId: RetrieveBusiness
      x-api-path-slug: v1me-get
      responses:
        200:
          description: OK
      tags:
      - Businesss
      - Information
  /v1/me/employees:
    get:
      summary: Provides summary information for all of a business's employees.
      description: Provides summary information for all of a business's employees.
      operationId: ListEmployees
      x-api-path-slug: v1meemployees-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_created_at
        description: If filtering results by their created_at field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: begin_updated_at
        description: If filtering results by their updated_at field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: end_created_at
        description: If filtering results by their created_at field, the end of the
          requested reporting period, in ISO 8601 format
      - in: query
        name: end_updated_at
        description: If filtering results by there updated_at field, the end of the
          requested reporting period, in ISO 8601 format
      - in: query
        name: external_id
        description: If provided, the endpoint returns only employee entities with
          the specified external_id
      - in: query
        name: limit
        description: The maximum integer number of employee entities to return in
          a single response
      - in: query
        name: order
        description: The order in which employees are listed in the response, based
          on their created_at field
      - in: query
        name: status
        description: If provided, the endpoint returns only employee entities with
          the specified status (ACTIVE or INACTIVE)
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Businesss
      - Employees
  /v1/me/roles:
    get:
      summary: Provides summary information for all of a business's employee roles.
      description: Provides summary information for all of a business's employee roles.
      operationId: ListEmployeeRoles
      x-api-path-slug: v1meroles-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum integer number of employee entities to return in
          a single response
      - in: query
        name: order
        description: The order in which employees are listed in the response, based
          on their created_at field
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Businesss
      - Employee
      - Roles
  /v1/me/timecards:
    get:
      summary: Provides summary information for all of a business's employee timecards.
      description: Provides summary information for all of a business's employee timecards.
      operationId: ListTimecards
      x-api-path-slug: v1metimecards-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_clockin_time
        description: If filtering results by their clockin_time field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: begin_clockout_time
        description: If filtering results by their clockout_time field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: begin_updated_at
        description: If filtering results by their updated_at field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: deleted
        description: If true, only deleted timecards are returned
      - in: query
        name: employee_id
        description: If provided, the endpoint returns only timecards for the employee
          with the specified ID
      - in: query
        name: end_clockin_time
        description: If filtering results by their clockin_time field, the end of
          the requested reporting period, in ISO 8601 format
      - in: query
        name: end_clockout_time
        description: If filtering results by their clockout_time field, the end of
          the requested reporting period, in ISO 8601 format
      - in: query
        name: end_updated_at
        description: If filtering results by their updated_at field, the end of the
          requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum integer number of employee entities to return in
          a single response
      - in: query
        name: order
        description: The order in which timecards are listed in the response, based
          on their created_at field
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Businesss
      - Employee
      - Timecards
  /v1/me/timecards/{timecard_id}:
    delete:
      summary: Deletes a timecard. Deleted timecards are still accessible from Connect
        API endpoints, but the value of their deleted field is set to true. See Handling
        deleted timecards for more information.
      description: Deletes a timecard. Deleted timecards are still accessible from
        Connect API endpoints, but the value of their deleted field is set to true.
        See Handling deleted timecards for more information.
      operationId: DeleteTimecard
      x-api-path-slug: v1metimecardstimecard-id-delete
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Timecard
      - ""
      - D
      - Timecards
      - Are
      - Still
      - Accessible
      - From
      - Connect
      - Endpoints
      - ""
      - But
      - Value
      - Of
      - Their
      - Deleted
      - Field
      - Is
      - Set
      - To
      - "True"
      - ""
      - See
      - Handling
      - Deleted
      - Timecardsmore
      - Information
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
  /v1/{location_id}/inventory:
    get:
      summary: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      description: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      operationId: ListInventory
      x-api-path-slug: v1location-idinventory-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of inventory entries to return in a single
          response
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Inventory
      - Information
      - Of
      - Merchants
      - Inventory-enabled
      - Item
      - Variations
  /v1/{location_id}/items:
    get:
      summary: Provides summary information for all of a location's items.
      description: Provides summary information for all of a location's items.
      operationId: ListItems
      x-api-path-slug: v1location-iditems-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: path
        name: location_id
        description: The ID of the location to list items for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Locations
      - Items
  /v1/{location_id}/payments:
    get:
      summary: Provides summary information for all payments taken by a merchant or
        any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      description: Provides summary information for all payments taken by a merchant
        or any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      operationId: ListPayments
      x-api-path-slug: v1location-idpayments-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list payments for
      - in: query
        name: order
        description: The order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Payments
      - Taken
      - By
      - Merchant
      - Any
      - Of
      - Merchants
      - Mobile
      - Staff
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
      - ""
      - See
      - Date
      - Rangesdetails
      - Of
      - Inclusive
      - Exclusive
      - Dates
  /v1/{location_id}/settlements:
    get:
      summary: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      description: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      operationId: ListSettlements
      x-api-path-slug: v1location-idsettlements-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list settlements for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      - in: query
        name: status
        description: Provide this parameter to retrieve only settlements with a particular
          status (SENT or FAILED)
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Deposits
      - Withdrawals
      - Initiated
      - By
      - Square
      - To
      - Merchants
      - Bank
      - Account
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
  /v1/{location_id}/orders:
    get:
      summary: Provides summary information for a merchant's online store orders.
      description: Provides summary information for a merchant's online store orders.
      operationId: ListOrders
      x-api-path-slug: v1location-idorders-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list online store orders for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Informationa
      - Merchants
      - Online
      - Store
      - Orders
  /v1/{location_id}/orders/{order_id}:
    get:
      summary: Provides comprehensive information for a single online store order,
        including the order's history.
      description: Provides comprehensive information for a single online store order,
        including the order's history.
      operationId: RetrieveOrder
      x-api-path-slug: v1location-idordersorder-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the orders associated location
      - in: path
        name: order_id
        description: The orders Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Online
      - Store
      - Order
      - ""
      - Including
      - Orders
      - History
  /v1/{location_id}/payments/{payment_id}:
    get:
      summary: Provides comprehensive information for a single payment.
      description: Provides comprehensive information for a single payment.
      operationId: RetrievePayment
      x-api-path-slug: v1location-idpaymentspayment-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the payments associated location
      - in: path
        name: payment_id
        description: The payments Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Payment
  /v1/{location_id}/settlements/{settlement_id}:
    get:
      summary: Provides comprehensive information for a single settlement, including
        the entries that contribute to the settlement's total.
      description: Provides comprehensive information for a single settlement, including
        the entries that contribute to the settlement's total.
      operationId: RetrieveSettlement
      x-api-path-slug: v1location-idsettlementssettlement-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the settlementss associated location
      - in: path
        name: settlement_id
        description: The settlements Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Settlement
      - ""
      - Including
      - Entries
      - That
      - Contribute
      - To
      - Settlements
      - Total
---