: MongoDB is a NoSQL database that stores data in a flexible, JSON-like format.

2. Q: How does MongoDB differ from relational databases?
   A: Unlike relational databases, MongoDB uses a document-oriented model with no fixed schema.

3. Q: What is a collection in MongoDB?
   A: A collection is a group of documents, similar to a table in relational databases.

4. Q: What is a document in MongoDB?
   A: A document is a JSON-like data structure that contains key-value pairs.

5. Q: What is the default database in MongoDB?
   A: The "test" database is the default database.

6. Q: What are indexes in MongoDB?
   A: Indexes improve query performance by allowing fast lookups of documents.

7. Q: How do you create an index in MongoDB?
   A: Use db.collection.createIndex({field: 1}) to create an index on a field.

8. Q: What is a primary key in MongoDB?
   A: The _id field is the primary key, and it uniquely identifies a document.

9. Q: How do you insert a document into a collection?
   A: Use db.collection.insertOne({name: "John"}) to insert a document.

10. Q: How do you insert multiple documents?
    A: Use db.collection.insertMany([{name: "John"}, {name: "Doe"}]).

11. Q: How do you retrieve all documents from a collection?
    A: Use db.collection.find() to fetch all documents.

12. Q: How do you retrieve specific fields in MongoDB?
    A: Use projection, e.g., db.collection.find({}, {name: 1, _id: 0}).

13. Q: How do you update a document in MongoDB?
    A: Use db.collection.updateOne({name: "John"}, {$set: {age: 30}}).

14. Q: How do you delete a document?
    A: Use db.collection.deleteOne({name: "John"}).

15. Q: What is the difference between find() and findOne()?
    A: find() returns multiple documents, while findOne() returns a single document.

16. Q: What is aggregation in MongoDB?
    A: Aggregation processes data and returns computed results, similar to SQL's GROUP BY.

17. Q: What is the use of $match in aggregation?
    A: $match filters documents based on conditions.

18. Q: What is $group used for in aggregation?
    A: $group is used to group documents and apply aggregate functions.

19. Q: How does MongoDB handle transactions?
    A: Transactions provide atomic operations on multiple documents across collections.

20. Q: What is sharding in MongoDB?
    A: Sharding partitions data across multiple servers to handle large datasets.

21. Q: What is replication in MongoDB?
    A: Replication creates multiple copies of data to ensure high availability.

22. Q: What is a replica set?
    A: A replica set is a group of MongoDB servers that maintain the same dataset.

23. Q: How do you create a backup of a MongoDB database?
    A: Use mongodump to create a backup and mongorestore to restore it.

24. Q: What is a capped collection?
    A: A capped collection is a fixed-size collection that automatically removes old documents.

25. Q: What is GridFS in MongoDB?
    A: GridFS is a storage mechanism for large files like images and videos.

26. Q: How do you increase write performance in MongoDB?
    A: Use indexing, sharding, and write concerns.

27. Q: How does MongoDB store data internally?
    A: MongoDB stores data in BSON format, which is a binary representation of JSON.

28. Q: What is $lookup in MongoDB?
    A: $lookup is used for performing JOIN-like operations in aggregation.

29. Q: What is the difference between $set and $push?
    A: $set updates a field, whereas $push adds elements to an array.

30. Q: How does MongoDB handle schema validation?
    A: MongoDB allows schema validation rules using JSON Schema.

31. Q: What is ObjectId in MongoDB?
    A: ObjectId is a unique identifier assigned to each document in MongoDB.

32. Q: What are TTL indexes?
    A: TTL (Time-To-Live) indexes automatically delete documents after a certain time.

33. Q: What is $unwind in aggregation?
    A: $unwind deconstructs an array field into multiple documents.

34. Q: How do you perform text search in MongoDB?
    A: Use text indexes and $text queries.

35. Q: What is a compound index?
    A: A compound index is an index on multiple fields.

36. Q: How do you perform geospatial queries in MongoDB?
    A: Use 2dsphere indexes and $geoWithin, $near queries.

37. Q: What is $out in aggregation?
    A: $out writes the aggregation result to a new collection.

38. Q: What is $merge in aggregation?
    A: $merge updates an existing collection with aggregation results.

39. Q: How does MongoDB handle concurrency?
    A: It uses locking mechanisms and optimistic concurrency control.

40. Q: What is $facet in aggregation?
    A: $facet allows multiple aggregations to be executed in a single query.

41. Q: What is $redact in aggregation?
    A: $redact filters document fields dynamically based on conditions.

42. Q: What are the advantages of using MongoDB?
    A: Scalability, flexibility, high availability, and ease of use.

43. Q: What are the disadvantages of MongoDB?
    A: Higher memory usage, lack of transactions in some cases, and no strict schema.

44. Q: How do you enable authentication in MongoDB?
    A: Use mongod --auth and create users with roles.

45. Q: What is $setIntersection?
    A: $setIntersection returns common elements from two arrays.

46. Q: What is $setUnion?
    A: $setUnion merges two arrays and removes duplicates.

47. Q: What is $setDifference?
    A: $setDifference returns elements present in one array but not in another.

48. Q: How do you handle large datasets in MongoDB?
    A: Use sharding, indexing, and aggregation optimization.

49. Q: What is $expr in MongoDB?
    A: $expr allows using aggregation expressions in queries.

50. Q: How do you improve query performance in MongoDB?
    A: Use indexing, proper schema design, and optimize aggregation pipelines.
