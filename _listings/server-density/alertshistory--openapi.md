---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: History API Listing costs
  description: |-
    Get the alerts history items limited by the given filter. If configId filter is set, then the results contains all events for that alert configuration. In any other case, the results are aggregated by itemId and configId including the following derived values:

    duration the sum of event durations.
    triggeredCount the number of events for that alert in that item.
    cost the HumanOps cost in seconds. For more information please check our support docs


    When the query is aggregated, the non-derived fields are from the document whose startDate is the newest. In addition to this, an unique id is generated by concatenating the itemId and the configId.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts/configs/subjectId:
    get:
      summary: Listing alerts by subject
      description: Get a list of all configured alerts for a specific subject (device
        or service).
      operationId: listing-alerts-by-subject
      x-api-path-slug: alertsconfigssubjectid-get
      parameters:
      - in: path
        name: subjectId
        description: The ID of the subject e
        type: string
      - in: path
        name: subjectType
        description: The type of the subject - device or service
        type: string
      - in: query
        name: subjectType
        description: The type of the subject - device or service
        type: string
      - in: path
        name: token
        description: Your API token
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/history/:
    "":
      summary: Listing costs
      description: |-
        Get the alerts history items limited by the given filter. If configId filter is set, then the results contains all events for that alert configuration. In any other case, the results are aggregated by itemId and configId including the following derived values:

        duration the sum of event durations.
        triggeredCount the number of events for that alert in that item.
        cost the HumanOps cost in seconds. For more information please check our support docs


        When the query is aggregated, the non-derived fields are from the document whose startDate is the newest. In addition to this, an unique id is generated by concatenating the itemId and the configId.
      operationId: listing-costs
      x-api-path-slug: alertshistory-
      parameters:
      - in: query
        name: configId
        description: _id of the config you want to limit by
        type: string
      - in: query
        name: end
        description: A string in the format, the end of the time frame eg
        type: string
      - in: query
        name: fields
        description: json encoded string - An array or a dict with all the fields
          we want returned
        type: string
      - in: query
        name: filter
        description: 'json encoded string - A dict with the filters we want to apply
          to the query (ex: {&quot;config'
        type: string
      - in: query
        name: order
        description: 'Sort ordering: ascending, descending'
        type: string
      - in: query
        name: page
        description: Page number, default = 1
        type: string
      - in: query
        name: perPage
        description: Documents that we&#39;re going to get per page
        type: string
      - in: query
        name: sort
        description: Field to sort by
        type: string
      - in: query
        name: start
        description: A string in the format, the beginning of the time frame eg
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        "":
          description: ""
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Alerts
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