# CLASS 03 READING DISCUSSION 
## Data Modeling & NoSQL Databases

#### 1. Why would a developer choose to make data models?
    - to create a structure around how data is stored and have checks built in to enforce that structure
#### 2. What purpose do CRUD operations serve?
    - to force actions to follow the defined structure of the data model
#### 3. What kind of database is Postgres? What kind of database is MongoDB?
    - Postgres is a SQL database. MongoDB is a NoSQL database. 
    - In a SQL database, everything belongs in defined tables 
    - NoSQL databases:
        - a system of IDs are used to find the data you're looking for
        - much more flexible than SQL databases
        - it can support changing nededs and can scale easily
#### 4. What is Mongoose and why do we need it?
    - Mongoose:
        - a package which translates our JavaScript into MongoDB
        - adds a lightweight structure and validity checking to our MongoDB to allow for some of the benefits of a SQL database
#### 5. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the contraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
    - Each person may or may not have a mother and a father and will have zero or more siblings. Each person will also have an occupation.
~~~
const personSchema = mongoose.Schema({
    name: { type: String, required: true },
    mother: { type: String, required: false },
    father: { type: String, required: false },
    siblings: { type: Number, required: true },
    occupation: { type: String, required: true },
});
~~~
