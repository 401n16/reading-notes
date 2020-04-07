# CLASS 08 READING DISCUSSION 
## Express Routing & Connected API

#### 1. What is a benefit to using *express.Router()*?
    Allows you to modularize your routes. Then, you can “use” them in your main server just like you would middleware. 
#### 2. When I say that top-down order matters in Express, what does that mean?
    Express executes code from top to bottom.
    Though Application Middleware is typically meant to be run before Handler Middleware, you can change this by moving an Application Middleware assignment after a Handler Middleware assignment. 
#### 3. Why do we use a model class (with *create()*, *read()*, etc.) instead of directly calling MongoDB operations (such as *save()*, *find()*, etc.) within our Express route handlers?
    Mongoose schema validation occurs with the Mongo Model.
    
