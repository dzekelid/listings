---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Remove Listing (by Seller)
  description: "Remove Listing (by Seller)<br/>\r\n- Seller cancels the market trade
    after listing but before bid/buy<br/>\r\n- Escrow from seller is returned back
    to the seller<br/>\r\n- End transaction state = Smart contract is rendered inactive<br/>"
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tradechain/ConfirmAbort:
    post:
      summary: Remove Listing (by Seller)
      description: "Remove Listing (by Seller)<br/>\r\n- Seller cancels the market
        trade after listing but before bid/buy<br/>\r\n- Escrow from seller is returned
        back to the seller<br/>\r\n- End transaction state = Smart contract is rendered
        inactive<br/>"
      operationId: TradechainConfirmAbortPost
      x-api-path-slug: tradechainconfirmabort-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      - in: formData
        name: itemSellerName
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Remove
      - Listing
      - (by
      - Seller)
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