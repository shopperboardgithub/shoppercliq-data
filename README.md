# ShopperCliq Product 

- Retrieve a list of products.
- Paginating results:  supports page size and page number, e.g. https://test.com/api/?limit=100&page=2

## Brand List

- Return brand list with products

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
                "description": "",
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
                                "additions": [
                                    {
                                        "name": "Testing",
                                        "price": 0
                                    },
                                    {
                                        "name": "Sub 1",
                                        "price": 12.84
                                    },
                                    {
                                        "name": "test 2",
                                        "price": 0
                                    },
                                    {
                                        "name": "sub 2",
                                        "price": 120
                                    }],
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

## Product Information

- Return single product information by product id

```JSON
{
    "id": 98345558566,
    "name": "Velvet Double Buckle Sling Back Heel",
    "price": 99,
    "usualPrice": 109,
    "image": "https://test.com/imageurl",
    "description": "",
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
                    "additions": [
                        {
                            "name": "Testing",
                            "price": 0
                        },
                        {
                            "name": "Sub 1",
                            "price": 12.84
                        },
                        {
                            "name": "test 2",
                            "price": 0
                        },
                        {
                            "name": "sub 2",
                            "price": 120
                        }],
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
```

## SKU Information

- Return single sku information by sku number

```JSON
{
    "id": 3434353443,
    "name": "36",
    "price": 199,
    "usualPrice": 199,
    "image": "https://test.com/imageurl2",
    "description": "",
    "skuNumber": "SH5310B214",
    "inventory": 999,
    "additions": [
        {
            "name": "Testing",
            "price": 0
        },
        {
            "name": "Sub 1",
            "price": 12.84
        },
        {
            "name": "test 2",
            "price": 0
        },
        {
            "name": "sub 2",
            "price": 120
        }],
    "variants": [
        {
            "name": "",
            "price": 199,
            "usualPrice": 199,
            "image": "https://test.com/imageurl"                                       
        }
    ]
}
```

## Properties

### Brand

| Name | Description | 
|------------|----------| 
| brandName | Brand name | 
| logo | Logo image URL | 
| banner | Banner image URL | 
| deliveryETA | Delivery information, e.g. After 72 hours | 
| geoLocation | Location information | 
| options | The custom product properties. For example, Size, Color, and Material. Product variants are made of up combinations of option values. | 

### Product

| Name | Description | 
|------------|----------| 
| id | An unique identifier for product |
| name | Product name |
| price | Product selling price. |
| usualPrice | Product usual price. |
| images | A list of product image |
| description | A list of description for the product, supports HTML formatting. Supports multiple type, e.g. shipping description, size description. | 
| option | The custom product properties. | 



 