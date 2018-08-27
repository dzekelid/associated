swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/products/{id}/modifiers/{id}/values/{id}/image:
    delete:
      summary: Delete the image associated with a modifier
      description: Delete the image applied to show when the modifier value is selected
      operationId: V3CatalogProductsModifiersIdValuesIdImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidmodifiersidvaluesidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Image
      - Associated
      - Modifier