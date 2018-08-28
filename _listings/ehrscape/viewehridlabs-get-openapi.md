---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Lab results
  description: Lab results.
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
paths:
  /view/{ehrId}/labs:
    get:
      summary: Lab results
      description: Lab results.
      operationId: get_labs
      x-api-path-slug: viewehridlabs-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Labs
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