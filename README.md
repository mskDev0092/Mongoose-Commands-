# Mongoosh Commands 

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

# mongoosh command to create:

> To create a document in Mongoose, you can use the create() method. This method takes a single argument, which is an object containing the data for the new document. For example:

```shell
MyModel.create({ name: 'John', age: 20 });
```

> This command will create a new document in the MyModel collection with the name property set to 'John' and the age property set to 20.

# mongoosh command to replace:

> To replace a document in Mongoose, you can use the findOneAndReplace() method. This method takes three arguments: a query object, a replacement document, and an optional options object. For example:

```shell
 MyModel.findOneAndReplace({ name: 'John' }, { name: 'Jane' }, { new: true });
```

> This command will search for a document with the name property of 'John' and replace it with a new document with the name property of 'Jane'. The { new: true } option will return the new document instead of the old one.

#  mongoosh command to update:

> The updateOne() method is a Mongoose function that updates a single document in a collection. It takes two arguments: a query object and an update object. The query object is used to identify the document to update, and the update object specifies the changes to be made. For example:

```shell
MyModel.updateOne({ name: 'John' }, { $set: { name: 'Jane' } });
```

> This command will search for the document with the name property of 'John' and replace it with a new document with the name property of 'Jane'.

# mongoosh command to delete:

> To delete documents in Mongoose, you can use the deleteOne() or deleteMany() methods. Both methods take a query object as an argument to identify the documents to delete. For example:

```shell
MyModel.deleteOne({ name: 'John' });
```

> This command will delete the document with the name property of 'John' from the MyModel collection.













































