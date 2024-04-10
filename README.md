## MongoDB Day1 Task

[Data Link](https://github.com/rvsp/database/blob/master/mongodb/product.json)

## For the following question write the corresponding MongoDB queries

1. Find all the information about each products

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find()`

```
[
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634b'),
    id: '1',
    product_name: 'Intelligent Fresh Chips',
    product_price: 655,
    product_material: 'Concrete',
    product_color: 'mint green'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634c'),
    id: '2',
    product_name: 'Practical Fresh Sausages',
    product_price: 911,
    product_material: 'Cotton',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634d'),
    id: '3',
    product_name: 'Refined Steel Car',
    product_price: 690,
    product_material: 'Rubber',
    product_color: 'gold'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634e'),
    id: '4',
    product_name: 'Gorgeous Plastic Pants',
    product_price: 492,
    product_material: 'Soft',
    product_color: 'plum'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634f'),
    id: '5',
    product_name: 'Sleek Cotton Chair',
    product_price: 33,
    product_material: 'Fresh',
    product_color: 'black'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6350'),
    id: '6',
    product_name: 'Awesome Wooden Towels',
    product_price: 474,
    product_material: 'Plastic',
    product_color: 'orange'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6351'),
    id: '7',
    product_name: 'Practical Soft Shoes',
    product_price: 500,
    product_material: 'Rubber',
    product_color: 'pink'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6352'),
    id: '8',
    product_name: 'Incredible Steel Hat',
    product_price: 78,
    product_material: 'Rubber',
    product_color: 'violet'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6353'),
    id: '9',
    product_name: 'Awesome Wooden Ball',
    product_price: 28,
    product_material: 'Soft',
    product_color: 'azure'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6354'),
    id: '10',
    product_name: 'Generic Wooden Pizza',
    product_price: 84,
    product_material: 'Frozen',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6355'),
    id: '11',
    product_name: 'Unbranded Wooden Cheese',
    product_price: 26,
    product_material: 'Soft',
    product_color: 'black'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6356'),
    id: '12',
    product_name: 'Unbranded Plastic Salad',
    product_price: 89,
    product_material: 'Wooden',
    product_color: 'pink'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6357'),
    id: '13',
    product_name: 'Gorgeous Cotton Keyboard',
    product_price: 37,
    product_material: 'Concrete',
    product_color: 'sky blue'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6358'),
    id: '14',
    product_name: 'Incredible Steel Shirt',
    product_price: 54,
    product_material: 'Metal',
    product_color: 'white'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6359'),
    id: '15',
    product_name: 'Ergonomic Cotton Hat',
    product_price: 43,
    product_material: 'Rubber',
    product_color: 'mint green'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635a'),
    id: '16',
    product_name: 'Small Soft Chair',
    product_price: 47,
    product_material: 'Cotton',
    product_color: 'teal'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635b'),
    id: '17',
    product_name: 'Incredible Metal Car',
    product_price: 36,
    product_material: 'Fresh',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635c'),
    id: '18',
    product_name: 'Licensed Plastic Bacon',
    product_price: 88,
    product_material: 'Steel',
    product_color: 'yellow'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635d'),
    id: '19',
    product_name: 'Intelligent Cotton Chips',
    product_price: 46,
    product_material: 'Soft',
    product_color: 'azure'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635e'),
    id: '20',
    product_name: 'Handcrafted Wooden Bacon',
    product_price: 36,
    product_material: 'Concrete',
    product_color: 'lime'
  }
]

```

2. Find the product price which are between 400 to 800

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({product_price: {$gte: 400, $lte:800}})`

```
[
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634b'),
    id: '1',
    product_name: 'Intelligent Fresh Chips',
    product_price: 655,
    product_material: 'Concrete',
    product_color: 'mint green'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634d'),
    id: '3',
    product_name: 'Refined Steel Car',
    product_price: 690,
    product_material: 'Rubber',
    product_color: 'gold'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634e'),
    id: '4',
    product_name: 'Gorgeous Plastic Pants',
    product_price: 492,
    product_material: 'Soft',
    product_color: 'plum'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6350'),
    id: '6',
    product_name: 'Awesome Wooden Towels',
    product_price: 474,
    product_material: 'Plastic',
    product_color: 'orange'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6351'),
    id: '7',
    product_name: 'Practical Soft Shoes',
    product_price: 500,
    product_material: 'Rubber',
    product_color: 'pink'
  }
]


```

3. Find the product price which are not between 400 to 600

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({$or: [{product_price: {$lt: 400}}, {product_price: {$gt:600}}]})`

```
[
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634b'),
    id: '1',
    product_name: 'Intelligent Fresh Chips',
    product_price: 655,
    product_material: 'Concrete',
    product_color: 'mint green'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634c'),
    id: '2',
    product_name: 'Practical Fresh Sausages',
    product_price: 911,
    product_material: 'Cotton',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634d'),
    id: '3',
    product_name: 'Refined Steel Car',
    product_price: 690,
    product_material: 'Rubber',
    product_color: 'gold'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef634f'),
    id: '5',
    product_name: 'Sleek Cotton Chair',
    product_price: 33,
    product_material: 'Fresh',
    product_color: 'black'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6352'),
    id: '8',
    product_name: 'Incredible Steel Hat',
    product_price: 78,
    product_material: 'Rubber',
    product_color: 'violet'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6353'),
    id: '9',
    product_name: 'Awesome Wooden Ball',
    product_price: 28,
    product_material: 'Soft',
    product_color: 'azure'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6354'),
    id: '10',
    product_name: 'Generic Wooden Pizza',
    product_price: 84,
    product_material: 'Frozen',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6355'),
    id: '11',
    product_name: 'Unbranded Wooden Cheese',
    product_price: 26,
    product_material: 'Soft',
    product_color: 'black'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6356'),
    id: '12',
    product_name: 'Unbranded Plastic Salad',
    product_price: 89,
    product_material: 'Wooden',
    product_color: 'pink'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6357'),
    id: '13',
    product_name: 'Gorgeous Cotton Keyboard',
    product_price: 37,
    product_material: 'Concrete',
    product_color: 'sky blue'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6358'),
    id: '14',
    product_name: 'Incredible Steel Shirt',
    product_price: 54,
    product_material: 'Metal',
    product_color: 'white'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6359'),
    id: '15',
    product_name: 'Ergonomic Cotton Hat',
    product_price: 43,
    product_material: 'Rubber',
    product_color: 'mint green'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635a'),
    id: '16',
    product_name: 'Small Soft Chair',
    product_price: 47,
    product_material: 'Cotton',
    product_color: 'teal'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635b'),
    id: '17',
    product_name: 'Incredible Metal Car',
    product_price: 36,
    product_material: 'Fresh',
    product_color: 'indigo'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635c'),
    id: '18',
    product_name: 'Licensed Plastic Bacon',
    product_price: 88,
    product_material: 'Steel',
    product_color: 'yellow'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635d'),
    id: '19',
    product_name: 'Intelligent Cotton Chips',
    product_price: 46,
    product_material: 'Soft',
    product_color: 'azure'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635e'),
    id: '20',
    product_name: 'Handcrafted Wooden Bacon',
    product_price: 36,
    product_material: 'Concrete',
    product_color: 'lime'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef635f'),
    id: '21',
    product_name: 'Unbranded Granite Chicken',
    product_price: 90,
    product_material: 'Metal',
    product_color: 'gold'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6360'),
    id: '22',
    product_name: 'Ergonomic Soft Hat',
    product_price: 99,
    product_material: 'Rubber',
    product_color: 'black'
  },
  {
    _id: ObjectId('66163f4fdfe91a24c5ef6361'),
    id: '23',
    product_name: 'Intelligent Steel Pizza',
    product_price: 95,
    product_material: 'Cotton',
    product_color: 'azure'
  }
]

```

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

5. Find the product name and product material of each products

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({}, {product_name: 1, product_price: 1})`

```
[
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4a9f'),
    product_name: 'Intelligent Fresh Chips',
    product_price: 655
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa0'),
    product_name: 'Practical Fresh Sausages',
    product_price: 911
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa1'),
    product_name: 'Refined Steel Car',
    product_price: 690
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa2'),
    product_name: 'Gorgeous Plastic Pants',
    product_price: 492
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa3'),
    product_name: 'Sleek Cotton Chair',
    product_price: 33
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa4'),
    product_name: 'Awesome Wooden Towels',
    product_price: 474
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa5'),
    product_name: 'Practical Soft Shoes',
    product_price: 500
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa6'),
    product_name: 'Incredible Steel Hat',
    product_price: 78
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa7'),
    product_name: 'Awesome Wooden Ball',
    product_price: 28
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa8'),
    product_name: 'Generic Wooden Pizza',
    product_price: 84
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa9'),
    product_name: 'Unbranded Wooden Cheese',
    product_price: 26
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aaa'),
    product_name: 'Unbranded Plastic Salad',
    product_price: 89
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aab'),
    product_name: 'Gorgeous Cotton Keyboard',
    product_price: 37
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aac'),
    product_name: 'Incredible Steel Shirt',
    product_price: 54
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aad'),
    product_name: 'Ergonomic Cotton Hat',
    product_price: 43
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aae'),
    product_name: 'Small Soft Chair',
    product_price: 47
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aaf'),
    product_name: 'Incredible Metal Car',
    product_price: 36
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4ab0'),
    product_name: 'Licensed Plastic Bacon',
    product_price: 88
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4ab1'),
    product_name: 'Intelligent Cotton Chips',
    product_price: 46
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4ab2'),
    product_name: 'Handcrafted Wooden Bacon',
    product_price: 36
  }
]

```

6. Find the product with a row id of 10

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({id: "10"})`

```
[
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa8'),
    id: '10',
    product_name: 'Generic Wooden Pizza',
    product_price: 84,
    product_material: 'Frozen',
    product_color: 'indigo'
  }
]


```

7. Find only the product name and product material

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({}, {_id: 0, product_name:1, product_material: 1})`

```
[
  {
    product_name: 'Intelligent Fresh Chips',
    product_material: 'Concrete'
  },
  {
    product_name: 'Practical Fresh Sausages',
    product_material: 'Cotton'
  },
  { product_name: 'Refined Steel Car', product_material: 'Rubber' },
  { product_name: 'Gorgeous Plastic Pants', product_material: 'Soft' },
  { product_name: 'Sleek Cotton Chair', product_material: 'Fresh' },
  {
    product_name: 'Awesome Wooden Towels',
    product_material: 'Plastic'
  },
  { product_name: 'Practical Soft Shoes', product_material: 'Rubber' },
  { product_name: 'Incredible Steel Hat', product_material: 'Rubber' },
  { product_name: 'Awesome Wooden Ball', product_material: 'Soft' },
  { product_name: 'Generic Wooden Pizza', product_material: 'Frozen' },
  { product_name: 'Unbranded Wooden Cheese', product_material: 'Soft' },
  {
    product_name: 'Unbranded Plastic Salad',
    product_material: 'Wooden'
  },
  {
    product_name: 'Gorgeous Cotton Keyboard',
    product_material: 'Concrete'
  },
  { product_name: 'Incredible Steel Shirt', product_material: 'Metal' },
  { product_name: 'Ergonomic Cotton Hat', product_material: 'Rubber' },
  { product_name: 'Small Soft Chair', product_material: 'Cotton' },
  { product_name: 'Incredible Metal Car', product_material: 'Fresh' },
  { product_name: 'Licensed Plastic Bacon', product_material: 'Steel' },
  {
    product_name: 'Intelligent Cotton Chips',
    product_material: 'Soft'
  },
  {
    product_name: 'Handcrafted Wooden Bacon',
    product_material: 'Concrete'
  }
]

```

8. Find all products which contain the value of soft in product material

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({"product_material": {"$regex": "soft", "$options": "i"}})`

or

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({product_material: /soft/i})`

```
[
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4ab1'),
    id: '19',
    product_name: 'Intelligent Cotton Chips',
    product_price: 46,
    product_material: 'Soft',
    product_color: 'azure'
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
    _id: ObjectId('66156ffa4b2c3fdb151f4aa7'),
    id: '9',
    product_name: 'Awesome Wooden Ball',
    product_price: 28,
    product_material: 'Soft',
    product_color: 'azure'
  },
  {
    _id: ObjectId('66156ffa4b2c3fdb151f4aa9'),
    id: '11',
    product_name: 'Unbranded Wooden Cheese',
    product_price: 26,
    product_material: 'Soft',
    product_color: 'black'
  }
]


```

9. Find products which contain product color indigo and product price 492.00

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.find({product_color:"indigo", product_price: "492.00"})`

    Products not available

10. Delete the products which product price value are 28

`Atlas atlas-11jmps-shard-0 [primary] Roadmap-Day35-Task> db.products.deleteMany({product_price: 28})`

```
{ acknowledged: true, deletedCount: 1 }

```
