swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 1
info:
  title: IDX API 1.4.0 Test Runner
  description: idx-broker-api-calls-in-version-1-4-0required-environment-variable-url-environment-variable-for-request-headers-environment-variable-partner-key-client-account-with-at-least-one-featured-listingtests-are-in-this-order-as-variables-such-as-listing-id-and-approved-mls-are-passed-to-subsequent-api-calls-
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
  /mls/prices/{approvedMLS}:
    get:
      summary: Get Mls Prices Approvedmls
      description: The sum total of properties listed in a given MLS as well as sums
        for each property type in the MLS.
      operationId: MlsPricesByApprovedMLSGet
      x-api-path-slug: mlspricesapprovedmls-get
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
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Prices
      - Approvedmls