1. Q: What is Mongoose in Node.js?
   A: Mongoose is an ODM (Object Data Modeling) library for MongoDB and Node.js that provides schema validation and query building.

2. Q: How do you install Mongoose in a Node.js project?
   A: Run npm install mongoose in the project directory.

3. Q: How do you connect to a MongoDB database using Mongoose?
   A: Use mongoose.connect('mongodb://localhost:27017/mydb', { useNewUrlParser: true, useUnifiedTopology: true });.

4. Q: What are Mongoose schemas?
   A: Mongoose schemas define the structure of documents in a collection, including fields, data types, and validation rules.

5. Q: How do you define a schema in Mongoose?
   A: Use const UserSchema = new mongoose.Schema({ name: String, age: Number });.

6. Q: What is a Mongoose model?
   A: A model is a constructor compiled from a schema that allows querying and modifying the database.

7. Q: How do you create a Mongoose model?
   A: Use const User = mongoose.model('User', UserSchema);.

8. Q: How do you insert a document using Mongoose?
   A: Use User.create({ name: 'John', age: 30 }); or new User({...}).save();.

9. Q: How do you retrieve all documents in a collection using Mongoose?
   A: Use User.find({}).

10. Q: How do you find a document by ID in Mongoose?
    A: Use User.findById(id).

11. Q: How do you update a document in Mongoose?
    A: Use User.findByIdAndUpdate(id, { age: 35 }, { new: true });.

12. Q: How do you delete a document in Mongoose?
    A: Use User.findByIdAndDelete(id);.

13. Q: What are Mongoose middlewares (pre and post hooks)?
    A: Functions that run before or after a document operation, like pre('save', function(next) { ... }).

14. Q: How do you add validation to a Mongoose schema?
    A: Use schema options like required: true or custom validators.

15. Q: How do you handle errors in Mongoose?
    A: Use .catch(err => console.error(err)); or try-catch blocks.

16. Q: What is population in Mongoose?
    A: Population allows referencing documents in other collections and fetching them automatically.

17. Q: How do you perform population in Mongoose?
    A: Use .populate('fieldName') in queries.

18. Q: What is a virtual field in Mongoose?
    A: A computed property that does not get stored in the database but is returned in queries.

19. Q: How do you define a virtual field?
    A: Use schema.virtual('fullName').get(function() { return this.firstName + ' ' + this.lastName; });.

20. Q: What is a Mongoose discriminator?
    A: A way to create multiple models with shared base schema while having different fields.

21. Q: How do you implement indexing in Mongoose?
    A: Use schema.index({ field: 1 }) to improve query performance.

22. Q: What are Mongoose instance methods?
    A: Custom functions on document instances, defined with schema.methods.

23. Q: How do you define a static method in Mongoose?
    A: Use schema.statics.findByName = function(name) { return this.find({ name }); }.

24. Q: What is the difference between lean() and normal queries?
    A: lean() returns plain JavaScript objects instead of Mongoose documents, improving performance.

25. Q: What is timestamps in Mongoose?
    A: timestamps: true automatically adds createdAt and updatedAt fields.

26. Q: How do you implement soft delete in Mongoose?
    A: Use deleted: Boolean instead of physically deleting records.

27. Q: What is toJSON in Mongoose?
    A: A transformation method for JSON serialization.

28. Q: How do you create a nested schema in Mongoose?
    A: Define subdocuments within a schema.

29. Q: What are findOneAndUpdate and findByIdAndUpdate?
    A: Methods for updating documents with options like { new: true } to return the updated document.

30. Q: How do you use transactions in Mongoose?
    A: Use MongoDB sessions with startSession() and commitTransaction().

31. Q: What is the purpose of useFindAndModify: false?
    A: It disables findAndModify, ensuring modern update methods are used.

32. Q: How do you handle connections in Mongoose?
    A: Use mongoose.connection.on('error', console.error);.

33. Q: What are aggregation pipelines in Mongoose?
    A: A way to process data in stages using User.aggregate([{ $match: {} }]).

34. Q: What is the difference between find() and aggregate()?
    A: find() retrieves documents, while aggregate() processes data in multiple steps.

35. Q: How do you limit query results in Mongoose?
    A: Use .limit(number). 

36. Q: What does distinct() do in Mongoose?
    A: It retrieves unique values of a field.

37. Q: How do you count documents in a collection?
    A: Use .countDocuments({}).

38. Q: How do you create a default value in Mongoose?
    A: Use default: value in schema definitions.

39. Q: What is the difference between validate and pre('save')?
    A: validate is for field validation, while pre('save') runs before saving.

40. Q: How do you sort query results?
    A: Use .sort({ field: 1 }) (ascending) or .sort({ field: -1 }) (descending).

41. Q: What is a capped collection in Mongoose?
    A: A fixed-size collection that automatically removes old data.

42. Q: How do you handle relationships in Mongoose?
    A: Using references (ref) or embedding documents.

43. Q: How do you implement full-text search in Mongoose?
    A: Use text indexes with schema.index({ field: 'text' }).

44. Q: What is Mongoose auto-increment?
    A: A plugin-based approach to automatically increment values.

45. Q: What is save() vs create()?
    A: save() applies to existing documents, while create() creates new ones.

46. Q: What is .exec() in Mongoose?
    A: It runs queries as Promises, improving performance.

47. Q: How do you handle bulk operations in Mongoose?
    A: Use bulkWrite([{ insertOne: {...} }, { updateOne: {...} }]).

48. Q: How do you prevent duplicate records in Mongoose?
    A: Use unique indexes like { field: { type: String, unique: true } }.

49. Q: How do you remove a field from a document in Mongoose?
    A: Use $unset: { field: 1 } in an update operation.

50. Q: What is the difference between updateOne() and updateMany()?
    A: updateOne() updates a single document, while updateMany() updates multiple documents.
