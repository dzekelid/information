---
swagger: "2.0"
x-collection-name: Coord
x-complete: 1
info:
  title: Users API
  description: the-users-api-allows-you-to-manage-user-data-on-the-coord-platform--sending-user-data-to-coordallows-you-to-perform-transactions-with-mobility-systems-like-renting-a-bike-parking-ina-parking-lot-or-booking-a-ridehail-trip-on-behalf-of-that-user-using-the-coord-platform-the-requirements-for-performing-a-transaction-for-a-given-user-vary-depending-on-the-systemyoure-connecting-with--some-systems-require-particular-data-about-a-user-in-order-for-thetransaction-to-take-place-and-some-systems-require-you-to-link-a-users-account--alltransactions-require-you-to-authenticate-the-user-using-a-jwt-every-coord-api-that-supports-transactions-has-an-endpoint-for-getting-information-aboutthat-apis-systems-along-with-what-you-need-to-provide-for-a-user-in-order-to-perform-atransaction-for-them--the-users-api-provides-tools-that-help-you-enable-users-to-performtransactions-as-well-as-tools-for-learning-about-the-transactions-that-a-user-can-alreadyperform-read-on-for-more-information-about-authenticating-users-linking-accounts-and-managing-userdata--authenticating-users-with-jwtsall-coord-api-endpoints-that-either-manipulate-data-or-perform-a-transaction-on-behalf-of-alogged-in-user-require-http-calls-to-include-an-authorization-bearer-jwt-token-so-thatthe-current-user-can-be-identified--all-endpoints-in-the-users-api-fall-into-this-categoryexcept-for-the-test-jwt-creation-endpoint-which-is-designed-to-allow-you-to-create-test-tokensfor-use-in-such-requests-for-information-on-how-to-create-nontest-user-authorization-tokensplease-contact-a-hrefmailtosalescoord-co-target-blanksalescoord-coaas-this-is-available-only-for-transaction-enabled-partners-see-post-v1userstestinguser-and-jwtreference0testjwtcreation-for-information-onhow-to-create-jwts-for-testing--linking-accountsmany-systems-require-you-to-link-a-user-in-order-to-perform-a-transaction--you-can-do-this-byredirecting-the-users-browser-or-webview-to-theget-v1userslink-accountreference0linkauseraccounttoenabletransactions-endpoint-this-will-allow-the-user-to-link-to-an-existing-account-with-that-system-if-they-have-one-orwill-create-a-new-one-for-them--if-you-call-this-endpoint-with-a-test-jwt-we-will-simulateaccount-linking-by-redirecting-the-user-to-a-demo-permission-page-you-can-also-simulate-linking-or-unlinking-test-users-accounts-serverside-by-calling-thepost-v1userstestingusercurrenttransactable-systemsreference0simulateaccountlinkingfortestingendpoint-remember-that-not-all-systems-are-transactable-and-not-all-transactable-systems-requireaccount-linking--getting-and-setting-user-infowe-automatically-ingest-user-information-like-email-addresses-and-names-from-the-jwtauthorization-token-you-send-us--information-about-a-users-vehicle-like-their-license-plateneeds-to-be-set-through-our-api--we-require-this-in-order-for-the-user-to-transact-with-certainparking-operators-you-can-call-get-v1usersusercurrentreference0getuserinfo-to-get-all-theinformation-we-have-about-a-user-including-the-fields-we-deduce-from-their-jwt-and-those-thatyou-have-already-set-through-our-api-you-can-call-v1usersusercurrentupdate-vehiclereference0updateuservehicle-toupdate-the-vehicle-thats-associated-with-a-users-account-
  version: 1.0.0
host: api.coord.co
basePath: /v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/current/stripe_info:
    post:
      summary: Update the user's stripe payment info
      description: |-
        Update the Stripe information associated with this user. You must call this endpoint in
        order for the current user to transact with a system that requires Stripe information. If
        this is the case, the system's transaction_info will contain
        `stripe_info.stripe_customer_id` in the `users_api_fields` array.

        Note that it's not possible to call this endpoint for test users (using a test JWT) and as
        such we do not support test transactions for any system with the
        stripe_info.stripe_customer_id requirement. If you are interested in transacting, please
        contact sales@coord.co.

        The request body must contain a Stripe token for this user that's targeted to Coord. You
        can do this either by tokenizing a new credit card on Stripe, or by generating a token from
        an existing Stripe customer in your system. In order to target the token to Coord, you must
        have already registered your Stripe account as a "platform" via Stripe Connect, and we must
        have accepted an invitation to connect to your platform. Assuming that has happened,
        you'll be able to generate coord-targeted tokens via an API call like the folllwing:

        Assuming your already have a customer with id `cus_abc` on your side:

        ```
        curl https://api.stripe.com/v1/tokens \
          -u sk_your_stripe_secret_key: \
          -d customer=cus_abc \
          -H "Stripe-Account: acct_coord_connected_account_id"
        ```

        Note the Stripe-Account header, which tells Stripe to create a token targeted to a specific
        connected account. You must always include that header and set its value to the ID of
        Coord's connected account, which you can find here: https://dashboard.stripe.com/applications/users.

        See https://stripe.com/docs/api#tokens for more info on Stripe tokens.

        ```
          {
            "coord_targeted_token": "tok_123"
          }
        ```

        On success, the response will be the identical object with a customer_id field set. This ID
        is the ID of the customer that Coord creates on Stripe.
        ```
          {
            "coord_targeted_token": "tok_123"
            "customer_id": "cus_xyz"
          }
        ```
      operationId: post_stripe_info
      x-api-path-slug: usercurrentstripe-info-post
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: body
        name: stripe_info
        description: A `StripeInfo` object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Stripe
      - Payment
      - Info
---