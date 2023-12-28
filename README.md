# ben-intro-project-backend
This is your repository for the Python server of your web application.

## Step 1: Database
You will store this data in a database - MySQL is a popular choice. On application start you will need to connect to the database, then on each API call query it to either read or write. This will require one table, called `Names`, that contains two columns: `name`, a `VARCHAR(20)`; and `count`, an `INTEGER`. 

- https://www.geeksforgeeks.org/python-database-tutorial/
- https://dev.mysql.com/doc/refman/8.0/en/data-types.html

## Step 2: Server
Create a server in Python that has 2 endpoints. Use this link for reference (I don't know Python sorry) https://realpython.com/api-integration-in-python/

- **POST** `/name` - this will increment a name in the database. Have it accept a JSON object such as `{ "name": "Squilliam" }`
- **GET** `/names` - this will return a list of the top 5 names. Have it return a JSON array like `[ { "name": "Squilliam", "count": 4 }, { "name": "Eugene", "count": 2 } ]`

Once you have the server running, you can use [Postman](https://www.postman.com/downloads/) to test your endpoints by making API calls. You could also use CURL or similar, but Postman has a GUI. Once you have that working, we can talk about frontend stuff and making a web form for this. The easiest thing is to just make an HTML form with some Javascript to call the API, but you can go more advanced to using React or Vue or whatever.
