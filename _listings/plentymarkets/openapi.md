swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/items/{id}/variations/{variationId}/stock/bookIncomingItems:
    put:
      summary: Book incoming stock
      description: Books incoming stock for a variation. The incoming stock will be
        added to the existing stock. The ID of the item and the ID of the variation
        must be specified.
      operationId: putRestItemsVariationsVariationStockBookincomingitems
      x-api-path-slug: restitemsidvariationsvariationidstockbookincomingitems-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/bookIncomingItems
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Incoming
      - Stock
  /rest/orders/{orderId}/outgoing_stocks:
    post:
      summary: Book out order items
      description: Books out the order items of an order. The ID of the order must
        be specified and a booking date can be specified. The current date and time
        will be used if no date is specified.
      operationId: postRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-post
      parameters:
      - in: query
        name: date
        description: The date that is saved as booking date for the outgoing stock
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Out
      - Order
      - Items
  /rest/stockmanagement/warehouses/{warehouseId}/stock/bookIncomingItems:
    put:
      summary: Book incoming stock
      description: Books incoming stock for multiple variations. The incoming stock
        will be added to the existing stock. The ID of the warehouse must be specified.
      operationId: putRestStockmanagementWarehousesWarehouseStockBookincomingitems
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockbookincomingitems-put
      parameters:
      - in: body
        name: /rest/stockmanagement/warehouses/{warehouseId}/stock/bookIncomingItems
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Incoming
      - Stock