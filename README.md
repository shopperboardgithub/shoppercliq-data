# ShopperBoard Product 

- Retrieve a list of products.
- Paginating results:  supports page size and page number, e.g. https://test.com/api/?limit=100&page=2

```JSON
[
    {
        "brandName": "",
        "companyName": "",
        "description": "",
        "logo": "",
        "banner": "",
        "deliveryETA": "Delivery information",
        "specialRemark": "",
        "phoneNumber": "",
        "address": "",
        "reference": "",
        "geoLocation": {
            "lat": 0,
            "lon": 0
        },
        "productList": [
            {
                "id": 98345558566,
                "name": "Velvet Double Buckle Sling Back Heel",
                "price": 99,
                "usualPrice": 109,
                "image": "https://test.com/imageurl",
                "desc": "",
                "images": [
                    "https://test.com/imageurl1",
                    "https://test.com/imageurl2"
                ],
                "categories": [
                    {
                        "id": 0,
                        "name": "Set Menu",
                        "skuList": [
                            {
                                "id": 3434353443,
                                "name": "36",
                                "price": 199,
                                "usualPrice": 199,
                                "image": "https://test.com/imageurl2",
                                "description": "",
                                "skuNumber": "SH5310B214",
                                "inventory": 999,
                                "variants": [
                                    {
                                        "name": "",
                                        "price": 199,
                                        "usualPrice": 199,
                                        "image": "https://test.com/imageurl"
                                    }
                                ]
                            }
                        ]
                    }
                ]
            }
        ]
    }
]
```


## Properties

### Product

| Name | Description | 
|------------|----------| 
| id | An unique identifier for product, number or string. |
| title | Product name |
| url | Product url |
| price | Product selling price. |
| usualPrice | Product usual price. |
| published_at | The date and time when the product was published. optional. |
| images | A list of product image |
| description | A list of description for the product, supports HTML formatting. Supports multiple type, e.g. shipping description, size description. |
| variants | The Product resource will have a variant for every possible combination of its options. Each product have a variant at least. |
| options | The custom product properties. For example, Size, Color, and Material. Product variants are made of up combinations of option values.|
 
### Variant

| Name | Description | 
|------------|----------| 
| id | An unique identifier for product, number or string. |
| sku | Product sku. |
| price | Product selling price. |
| usualPrice | Product usual price. |
| grams | The weight of the product variant in grams. |  
| images | A list of product image, optional. |
| quantity | Product inventory |
| option | The custom product properties. |
