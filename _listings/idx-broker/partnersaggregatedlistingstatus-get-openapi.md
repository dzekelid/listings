---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Get Partners Aggregated Listing Status
  description: This method gives the status for all MLS listings (not supplemental)
    broken down by client account ID. This includes sold/pending listings with an
    unknown status which are not usually returned by sold/pending api methods. This
    is helpful if you need to know when previously gathered featured properties have
    left the market.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clients/listing/{approvedMLS}/{featuredId}:
    get:
      summary: Get Listing Approved MLS Featuredid
      description: Returns the detailed information for a given listingID.
      operationId: ClientsListingByApprovedMLSAndFeaturedIdGet
      x-api-path-slug: clientslistingapprovedmlsfeaturedid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: path
        name: featuredId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Approved
      - MLS
      - Featuredid
  /partners/aggregatedlistingstatus:
    get:
      summary: Get Partners Aggregated Listing Status
      description: This method gives the status for all MLS listings (not supplemental)
        broken down by client account ID. This includes sold/pending listings with
        an unknown status which are not usually returned by sold/pending api methods.
        This is helpful if you need to know when previously gathered featured properties
        have left the market.
      operationId: PartnersAggregatedlistingstatusGet
      x-api-path-slug: partnersaggregatedlistingstatus-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Listing
      - Status
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