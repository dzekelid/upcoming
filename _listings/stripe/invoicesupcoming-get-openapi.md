---
swagger: "2.0"
x-collection-name: Stripe
x-complete: 0
info:
  title: Stripe Get Invoices Upcoming
  description: At any time, you can preview the upcoming invoice for a customer. This
    will show you all the charges that are pending, including subscription renewal
    charges, invoice item charges, etc. It will also show you any discount that is
    applicable to the customer.Note that when you are viewing an upcoming invoice,
    you are simply viewing a preview ??? the invoice has not yet been created. As
    such, the upcoming invoice will not show up in invoice listing calls, and you
    cannot use the API to pay or edit the invoice. If you want to change the amount
    that your customer will be billed, you can add, remove, or update pending invoice
    items, or update the customer???s discount.You can preview the effects of updating
    a subscription, including a preview of what proration will take place. To ensure
    that the actual proration is calculated exactly the same as the previewed proration,
    you should pass a proration_date parameter when doing the actual subscription
    update. The value passed in should be the same as the subscription_proration_date
    returned on the upcoming invoice resource. The recommended way to get only the
    prorations being previewed is to consider only proration line items where period[start]
    is equal to the subscription_proration_date on the upcoming invoice resource.
  termsOfService: https://stripe.com/us/terms/
  contact:
    name: Stripe Dev Platform Team
    url: https://stripe.com
    email: dev-platform@stripe.com
  version: v1
host: api.stripe.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /invoices/upcoming:
    get:
      summary: Get Invoices Upcoming
      description: At any time, you can preview the upcoming invoice for a customer.
        This will show you all the charges that are pending, including subscription
        renewal charges, invoice item charges, etc. It will also show you any discount
        that is applicable to the customer.Note that when you are viewing an upcoming
        invoice, you are simply viewing a preview ??? the invoice has not yet been
        created. As such, the upcoming invoice will not show up in invoice listing
        calls, and you cannot use the API to pay or edit the invoice. If you want
        to change the amount that your customer will be billed, you can add, remove,
        or update pending invoice items, or update the customer???s discount.You can
        preview the effects of updating a subscription, including a preview of what
        proration will take place. To ensure that the actual proration is calculated
        exactly the same as the previewed proration, you should pass a proration_date
        parameter when doing the actual subscription update. The value passed in should
        be the same as the subscription_proration_date returned on the upcoming invoice
        resource. The recommended way to get only the prorations being previewed is
        to consider only proration line items where period[start] is equal to the
        subscription_proration_date on the upcoming invoice resource.
      operationId: getInvoicesUpcoming
      x-api-path-slug: invoicesupcoming-get
      parameters:
      - in: query
        name: coupon
        description: The code of the coupon to apply
      - in: query
        name: customer
        description: The identifier of the customer whose upcoming invoice youd like
          to retrieve
      - in: query
        name: expand
        description: Specifies which fields in the response should be expanded
      - in: query
        name: invoice_items
        description: List of invoice items to add or update in the upcoming invoice
          preview
      - in: query
        name: subscription
        description: The identifier of the subscription for which youd like to retrieve
          the upcoming invoice
      - in: query
        name: subscription_items
        description: List of subscription items, each with an attached plan
      - in: query
        name: subscription_prorate
        description: If previewing an update to a subscription, this decides whether
          the preview will show the result of applying prorations or not
      - in: query
        name: subscription_proration_date
        description: If previewing an update to a subscription, and doing proration,
          `subscription_proration_date` forces the proration to be calculated as though
          the update was done at the specified time
      - in: query
        name: subscription_tax_percent
        description: If provided, the invoice returned will preview updating or creating
          a subscription with that tax percent
      - in: query
        name: subscription_trial_end
        description: If provided, the invoice returned will preview updating or creating
          a subscription with that trial end
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Invoices
      - Upcoming
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