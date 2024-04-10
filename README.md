## MongoDB Day1 Task

[Data Link](https://github.com/rvsp/database/blob/master/mongodb/product.json)

## For the following question write the corresponding MongoDB queries

1. Find all the information about each products

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find()`

2. Find the product price which are between 400 to 800

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({product_price: {$gte: 400, $lte:800}})
[
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4a9f'),
    id: '1',
    product_name: 'Intelligent Fresh Chips',
    product_price: 655,
    product_material: 'Concrete',
    product_color: 'mint green'
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa1'),
    id: '3',
    product_name: 'Refined Steel Car',
    product_price: 690,
    product_material: 'Rubber',
    product_color: 'gold'
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa2'),
    id: '4',
    product_name: 'Gorgeous Plastic Pants',
    product_price: 492,
    product_material: 'Soft',
    product_color: 'plum'
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa4'),
    id: '6',
    product_name: 'Awesome Wooden Towels',
    product_price: 474,
    product_material: 'Plastic',
    product_color: 'orange'
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa5'),
    id: '7',
    product_name: 'Practical Soft Shoes',
    product_price: 500,
    product_material: 'Rubber',
    product_color: 'pink'
  }
]
`
