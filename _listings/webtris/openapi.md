---
swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: webtris.highwaysengland.co.uk
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/areas/{area_Ids}:
    get:
      summary: Returns details of selected area
      description: Returns details of selected area.
      operationId: Areas_Get
      x-api-path-slug: vversionareasarea-ids-get
      parameters:
      - in: path
        name: area_Ids
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Details
      - Of
      - Selected
      - Area
  /v{version}/sites/{site_Ids}:
    get:
      summary: Get selected sites
      description: Get selected sites.
      operationId: Sites_Index
      x-api-path-slug: vversionsitessite-ids-get
      parameters:
      - in: path
        name: site_Ids
        description: site id
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Selected
      - Sites
---