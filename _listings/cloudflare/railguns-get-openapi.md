---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare List, search, sort and filter your Railguns
  version: 1.0.0
  description: List, search, sort and filter your Railguns
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /railguns:
    get:
      summary: List, search, sort and filter your Railguns
      description: List, search, sort and filter your Railguns
      operationId: cloudflare-railgun-api
      x-api-path-slug: railguns-get
      parameters:
      - in: query
        name: direction
        description: Direction to order Railgunsttttttttttttttdesc
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of items per pagetttttttttttttt20
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Performance
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