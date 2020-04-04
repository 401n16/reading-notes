# CLASS 07 READING DISCUSSION 
## Express Server

#### 1. What code does the server actually run?
    middleware
#### 2. What Express/HTTP operations map to CRUD operations?
    Create = Post
    Read = Get
    Update = Put
    Delete = Delete
#### 3. What does *res.send()* do?
    res.send() sends something as the response to the client
#### 4. What is the order of operations for the three categories of middleware (handler, application, route)?
    route
    handler
    application
#### 5. What is the parameter *next* used for?
    calls the next middleware in the chain
