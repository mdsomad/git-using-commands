# All MongoDb commands you will ever need (MongoDb Cheatsheet)


- First commant
```sh
 mongo
```


## 1. Database Commands
- View all databases
```sh
flutter build appbundle
```

- Create a new or switch databases 
```sh
use dbName
```

- View current Database 
```sh
db
```

- Delete Database 
```sh
db.dropDatabase()
```

## 2. Collection Commands
- All Show & View Collections
```sh
 show collections
```

- Create a collection named 'comments'
```sh
 db.createCollection('comments')
```

- Drop & Delete a collection named 'comments'
```sh
 db.comments.drop()
```

## 3. Row(Document) Commands
- Show & view all Rows in a Collection named example this --> comments
```sh
 db.comments.find()
```

- Show all Rows in a Collection (Prettified) (Rows ko Behtarin Tarike se Show & View karta hai ) (or yah hai Collection ko named --> comments)
```sh
 db.comments.find().pretty()
```

- Find the first row matching the object  ( Only Single Row Find or yah hai Collection ko named --> comments)
```sh
db.comments.findOne({name: 'Somad'})
```

- Insert One Row  ( Only Single Row Add & Insert or yah hai Collection ko named --> comments )
```sh
db.comments.insert({
    'name': 'Somad',
    'lang': 'JavaScript',
    'member_since': 5
 })
```

- Insert many Rows  ( Multiple Rows Add & Insert or yah hai Collection ko named --> comments )
```sh
db.comments.insertMany([{
    'name': 'Somad',
    'lang': 'dart & JavaScript',
    'member_since': 5
    }, 
    {'name': 'yasin',
    'lang': 'JavaScript',
    'member_since': 3
    },
    {'name': 'alif',
    'lang': 'dart',
    'member_since': 3
    },
    {'name': 'abul',
    'lang': 'C#',
    'member_since': 4
}])
```

- Search in a MongoDb Database  (yah hai Collection ko named --> comments)
```sh
db.comments.find({lang:'dart'})
```

- Limit the number of rows in output  (yah hai Collection ko named --> comments) (limit(2) Matlab ya hai First ka do Rows hi sirf show & view Karega or app apna hisab kabhi number de sakte hai)
```sh
db.comments.find().limit(2)
```

- Count the number of rows in the output  (yah hai Collection ko named --> comments) (count() Matlab ya hai is Collection Mein Total Kitna Rows hai yahi Batata hai )
```sh
db.comments.find().count()
```

- Update a row  (yah hai Collection ko named --> comments) ({upsert: true} <-- Karne se yah row Agar Nahin hai Database Mein to yah add kar dega)
```sh
db.comments.updateOne({name:'akif'},
{$set: {'name': 'subhan',
    'lang': 'JavaScript',
    'member_since': 51
}}, {upsert: true})
```

- Mongodb Increment Operator  (yah hai Collection ko named --> comments) 
```sh
db.comments.update({name: 'yasin'},
{$inc:{
    member_since: 2
}})
```

- Mongodb Rename Operator  (yah hai Collection ko named --> comments) 
```sh
db.comments.update({name: 'akif'},
{$rename:{
    member_since: 'member'
}})
```

- Delete Row   (yah hai Collection ko named --> comments) 
```sh
db.comments.remove({name: 'abul'})
```

- Less than/Greater than/ Less than or Eq/Greater than or Eq   (yah hai Collection ko named --> comments) 
```sh
db.comments.find({member_since: {$lt: 90}})
```

```sh
db.comments.find({member_since: {$lte: 90}})
```

```sh
db.comments.find({member_since: {$gt: 90}})
```

```sh
db.comments.find({member_since: {$gte: 90}})
```

