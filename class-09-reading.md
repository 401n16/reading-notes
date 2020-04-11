# CLASS 09 READING DISCUSSION 
## API Server

#### 1. Describe a use-case where param middleware would come in handy.
    The ability to add specific middleware depending on if req.params has a key-value set can be used to validate or formatthe req.params key-value before that value is consumed by a GET, POST, PUT, or DELETE route.
#### 2. What are the two ways to add middleware in-between Mongoose and MongoDB interactions?
    populate() or virtual joins
#### 3. What is the difference between a join by reference and a virtual join?
        I think they are the same thing.
#### 4. What do *localField* and *foreignField* mean?
    Fields in the current collection or an outside collection.

    
