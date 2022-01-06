# ShopperCliq Product 

- Retrieve Brand and Product information
- Total 3 apis: Brand List, Product Information and SKU Information
- Paginating results: supports page size and page number, e.g. https://test.com/api/?limit=100&page=2

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
                                "name": "name123",
                                "price": 199,
                                "usualPrice": 199,
                                "image": "https://test.com/imageurl2",
                                "description": "",
                                "skuNumber": "SH5310B214",
                                "inventory": 999,
                                "addOns": [
                                    {
                                        "name": "Choice of Soft Drink / Slushie",
                                        "maxSelect": 1,
                                        "choices": [
                                            { "name": "Coke", "priceAdjustment": 0.00 },
                                            { "name" : "Coke Zero", "priceAdjustment": 0.00 },
                                            { "name": "100 Plus", "priceAdjustment": 0.00 },
                                            { "name" : "OFC Golden Lime Slushie", "priceAdjustment": 0.00 }
                                        ]
                                    },
                                    {
                                        "name": "Choice of Fries",
                                        "maxSelect": 1,
                                        "choices": [
                                            { "name": "Regular fries", "priceAdjustment": 0.00 },
                                            { "name": "Upgrade to Cheese fries", "priceAdjustment": 2.00 },
                                            { "name" : "Upgrade to Truffle fries", "priceAdjustment": 2.50 }
                                        ]
                                    },
                                    {
                                        "name": "Extra Beef Patty",
                                        "maxSelect": 1,
                                        "choices": [
                                            { "name": "Add one beef patty", "priceAdjustment": 8.00 },
                                            { "name": "Add two beef patties", "priceAdjustment": 16.00 }
                                        ]
                                    },
                                    {
                                        "name": "Extra Cheese",
                                        "maxSelect": 1,
                                        "choices": [
                                            { "name": "Add one cheese", "priceAdjustment": 1.00 },
                                            { "name": "Add two cheese", "priceAdjustment": 2.00 }
                                        ]
                                    },
                                    {
                                        "name": "Extra Tomato",
                                        "maxSelect": 1,
                                        "choices": [
                                            { "name": "Add one tomato", "priceAdjustment": 8.00 },
                                            { "name": "Add two tomatoes", "priceAdjustment": 16.00 }
                                        ]
                                    }
                                ],
                                "variants": [
                                    {
                                        "id": 8989,
                                        "name": "name123 - White (Medium)",
                                        "price": 199,
                                        "usualPrice": 199,
                                        "image": "https://test.com/imageurl",
                                        "options": [
                                            { "name": "Color", "choice": "White" },
                                            { "name": "Size", "choice": "Medium" }
                                        ],
                                        "inventory": 999                                  
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
                    "name": "name123",
                    "price": 199,
                    "usualPrice": 199,
                    "image": "https://test.com/imageurl2",
                    "description": "",
                    "skuNumber": "SH5310B214",
                    "inventory": 999,
                    "addOns": [
                        {
                            "name": "Choice of Soft Drink / Slushie",
                            "maxSelect": 1,
                            "choices": [
                                { "name": "Coke", "priceAdjustment": 0.00 },
                                { "name" : "Coke Zero", "priceAdjustment": 0.00 },
                                { "name": "100 Plus", "priceAdjustment": 0.00 },
                                { "name" : "OFC Golden Lime Slushie", "priceAdjustment": 0.00 }
                            ]
                        },
                        {
                            "name": "Choice of Fries",
                            "maxSelect": 1,
                            "choices": [
                                { "name": "Regular fries", "priceAdjustment": 0.00 },
                                { "name": "Upgrade to Cheese fries", "priceAdjustment": 2.00 },
                                { "name" : "Upgrade to Truffle fries", "priceAdjustment": 2.50 }
                            ]
                        },
                        {
                            "name": "Extra Beef Patty",
                            "maxSelect": 1,
                            "choices": [
                                { "name": "Add one beef patty", "priceAdjustment": 8.00 },
                                { "name": "Add two beef patties", "priceAdjustment": 16.00 }
                            ]
                        },
                        {
                            "name": "Extra Cheese",
                            "maxSelect": 1,
                            "choices": [
                                { "name": "Add one cheese", "priceAdjustment": 1.00 },
                                { "name": "Add two cheese", "priceAdjustment": 2.00 }
                            ]
                        },
                        {
                            "name": "Extra Tomato",
                            "maxSelect": 1,
                            "choices": [
                                { "name": "Add one tomato", "priceAdjustment": 8.00 },
                                { "name": "Add two tomatoes", "priceAdjustment": 16.00 }
                            ]
                        }
                    ],
                    "variants": [
                        {
                            "id": 8989,
                            "name": "name123 - White (Medium)",
                            "price": 199,
                            "usualPrice": 199,
                            "image": "https://test.com/imageurl",
                            "options": [
                                { "name": "Color", "choice": "White" },
                                { "name": "Size", "choice": "Medium" }
                            ],
                            "inventory": 999                                  
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
    "name": "name123",
    "price": 199,
    "usualPrice": 199,
    "image": "https://test.com/imageurl2",
    "description": "",
    "skuNumber": "SH5310B214",
    "inventory": 999,
    "addOns": [
        {
            "name": "Choice of Soft Drink / Slushie",
            "maxSelect": 1,
            "choices": [
                { "name": "Coke", "priceAdjustment": 0.00 },
                { "name" : "Coke Zero", "priceAdjustment": 0.00 },
                { "name": "100 Plus", "priceAdjustment": 0.00 },
                { "name" : "OFC Golden Lime Slushie", "priceAdjustment": 0.00 }
            ]
        },
        {
            "name": "Choice of Fries",
            "maxSelect": 1,
            "choices": [
                { "name": "Regular fries", "priceAdjustment": 0.00 },
                { "name": "Upgrade to Cheese fries", "priceAdjustment": 2.00 },
                { "name" : "Upgrade to Truffle fries", "priceAdjustment": 2.50 }
            ]
        },
        {
            "name": "Extra Beef Patty",
            "maxSelect": 1,
            "choices": [
                { "name": "Add one beef patty", "priceAdjustment": 8.00 },
                { "name": "Add two beef patties", "priceAdjustment": 16.00 }
            ]
        },
        {
            "name": "Extra Cheese",
            "maxSelect": 1,
            "choices": [
                { "name": "Add one cheese", "priceAdjustment": 1.00 },
                { "name": "Add two cheese", "priceAdjustment": 2.00 }
            ]
        },
        {
            "name": "Extra Tomato",
            "maxSelect": 1,
            "choices": [
                { "name": "Add one tomato", "priceAdjustment": 8.00 },
                { "name": "Add two tomatoes", "priceAdjustment": 16.00 }
            ]
        }
    ],
    "variants": [
        {
            "id": 8989,
            "name": "name123 - White (Medium)",
            "price": 199,
            "usualPrice": 199,
            "image": "https://test.com/imageurl",
            "options": [
                { "name": "Color", "choice": "White" },
                { "name": "Size", "choice": "Medium" }
            ],
            "inventory": 999                                  
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

### Product

| Name | Description | 
|------------|----------| 
| id | An unique identifier for product |
| name | Product name |
| price | Product selling price. |
| usualPrice | Product usual price. |
| images | A list of product image |
| description | A list of description for the product, supports HTML formatting. Supports multiple type, e.g. shipping description, size description. | 



 