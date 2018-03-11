---
swagger: "2.0"
info:
  title: Blockchain Info
  description: Use Blockchain's APIs at no cost to help you start building bitcoin
    apps.
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rawblock/{block_hash}:
    get:
      summary: Raw Block
      description: Returns a single raw block
      operationId: getRawBlock
      parameters:
      - in: path
        name: block_hash
        description: The block hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - blockchain
      - blocks
definitions: []
x-collection-name: Blockchain Info
x-streamrank:
  polling_total_time_average: "2.07"
  polling_size_download_average: "5152072.38"
  streaming_total_time_average: "1.19"
  streaming_size_download_average: "2602667.95"
  change_yes: "214"
  change_no: "1263"
  time_percentage: "43"
  size_percentage: "49"
  change_percentage: "14"
  last_run: "2018-02-21"
  days_run: "1"
  minute_run: "0"
---