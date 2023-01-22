# Mongoose Commands 

> Mongoose provides a few methods for performing data manipulation operations. These include:

```shell
    find() - Finds one or more documents in a collection.
```

```shell
    findOne() - Finds a single document in a collection.
```

```shell
    findOneAndUpdate() - Finds a single document and updates it.
```

```shell
    updateOne() - Updates a single document in a collection.
```

```shell
    updateMany() - Updates multiple documents in a collection.
```

```shell
    deleteOne() - Deletes a single document in a collection.
```

```shell
    deleteMany() - Deletes multiple documents in a collection.
```

```shell
    countDocuments() - Counts the number of documents in a collection.
```

```shell
    create() - Creates a new document in a collection.
```

```shell
   findOneAndReplace() - Replaces the entire document.
```

> The difference between the replace command and the update command in MongoDB is that the replace command replaces the entire document, while the update command only replaces or updates specific fields in the existing document. The replace command can be used if you want to replace the entire document with a new one, while the update command should be used if you only want to modify certain fields of an existing document.

# mongoose command find():

> To find documents in Mongoose, you can use the find() or findOne() methods. Both methods take a query object as an argument to identify the documents to find. For example:

```shell
MyModel.find({ name: 'John' });
```

> This command will search for documents with the name property of 'John' in the MyModel collection.

# mongoose command findOne():

> To find a single document in Mongoose, you can use the findOne() method. It takes a query object as an argument to identify the document to find. For example:

```shell
MyModel.findOne({ name: 'John' });
```

> This command will search for the document with the name property of 'John' in the MyModel collection.

# mongoose command findOneAndUpdate():

> To update a single document in Mongoose, you can use the findOneAndUpdate() method. It takes a query object and an update object as arguments to identify the document to update and the values to update it with. For example:

```shell
MyModel.findOneAndUpdate({ name: 'John' }, { age: 21 });
```

> This command will update the document with the name property of 'John' in the MyModel collection to have the age property set to 21.

# mongoose command updateOne():

> To update a single document in Mongoose, you can use the updateOne() method. It takes a query object and an update object as arguments to identify the document to update and the values to update it with. For example:

```shell
MyModel.updateOne({ name: 'John' }, { age: 21 });
```

> This command will update the document with the name property of 'John' in the MyModel collection to have the age property set to 21.

# mongoose command updateMany():

> To update multiple documents in Mongoose, you can use the updateMany() method. It takes a query object and an update object as arguments to identify the documents to update and the values to update them with. For example:

```shell
MyModel.updateMany({ age: { $lt: 21 } }, { age: 21 });
```

> This command will update all documents in the MyModel collection whose age property is less than 21 to have the age property set to 21.

# mongoose command deleteOne():

> To delete documents in Mongoose, you can use the deleteOne() or deleteMany() methods. Both methods take a query object as an argument to identify the documents to delete. For example:

```shell
MyModel.deleteOne({ name: 'John' });
```

> This command will delete the document with the name property of 'John' from the MyModel collection.

# mongoose command deleteMany()

> To delete multiple documents in Mongoose, you can use the deleteMany() method. It takes a query object as an argument to identify the documents to delete. For example:

```shell
MyModel.deleteMany({ age: { $lt: 21 } });
```

> This command will delete all documents in the MyModel collection whose age property is less than 21.

# mongoose command countDocuments():

> To count the number of documents in Mongoose, you can use the countDocuments() method. It takes a query object as an argument to identify the documents to count. For example:

```shell
MyModel.countDocuments({ age: { $lt: 21 } });
```

> This command will count the number of documents in the MyModel collection whose age property is less than 21.

# mongoose command create():

> To create a document in Mongoose, you can use the create() method. This method takes a single argument, which is an object containing the data for the new document. For example:

```shell
MyModel.create({ name: 'John', age: 20 });
```

> This command will create a new document in the MyModel collection with the name property set to 'John' and the age property set to 20.

# mongoose command findOneAndReplace():

> To replace a document in Mongoose, you can use the findOneAndReplace() method. This method takes three arguments: a query object, a replacement document, and an optional options object. For example:

```shell
 MyModel.findOneAndReplace({ name: 'John' }, { name: 'Jane' }, { new: true });
```

> This command will search for a document with the name property of 'John' and replace it with a new document with the name property of 'Jane'. The { new: true } option will return the new document instead of the old one.

















































