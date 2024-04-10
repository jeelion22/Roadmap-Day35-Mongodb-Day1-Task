## MongoDB Day1 Task

[Data Link](https://github.com/rvsp/database/blob/master/mongodb/product.json)

## For the following question write the corresponding MongoDB queries

1. Find all the information about each products

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find()`

2. Find the product price which are between 400 to 800

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({product_price: {$gte: 400, $lte:800}})`

3. Find the product price which are not between 400 to 600

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({$or: [{product_price: {$lt: 400}}, {product_price: {$gt:600}}]})`

4. List the four product which are greater than 500 in price

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({product_price: {$gt:500}}).limit(4)`

```
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
    _id: ObjectId('66156ffa4b2c3fdb151f4aa0'),
    id: '2',
    product_name: 'Practical Fresh Sausages',
    product_price: 911,
    product_material: 'Cotton',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa1'),
    id: '3',
    product_name: 'Refined Steel Car',
    product_price: 690,
    product_material: 'Rubber',
    product_color: 'gold'
  }
]

```
