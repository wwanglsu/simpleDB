# simpleDB
simulate the simple database using JavaScript, running on NodeJS.

Support Command Line comminucation with the database.

First Version: \n 
The database is running on the memory. Support the commands like: \n 
SET variable value
GET variable
NUMEQUALTO value

BEIGN
TRANSACT
SET variable value
GET variable
NUMEQUALTO value
COMMIT
ROLLBACK
END

Second Version, more work will be put on how to make the data more safe when memory crashes. 
<br><br><hr>
<h2>Knowledge abot MongoDB<h2>
<ul>What is MongoDB
  <li>Document Store</li>
  <li>Most popular document store, according to db-engines.com showing</li>
  <li>Designed for ease of development and scaling</li>
  <li>Supported by numerous programming languages</li>
  <li>Developed by 10gen in 2007</li>
</ul>
<br>
<ul>Main features of MongoDB
    <li>Ad-hoc queries.(namely "on the fly query",which is a query that cannot be determined prior to the moment the query is issued.<br> e.g. var queryStr="select * from table wherhe id="+myId . It is an entirely different query each time the line code is executed depending on the value of myId. The opposite of an Ad-hoc query <br>is a predefined query like Stored Procedure, where you have created a single query for the entire generalized<br> purpose of selecting fron that table and pass the ID as a variable.)</li>
    <li>Indexing and Secondary Indexing</li>
    <li>Replication</li>
    <li>Sharding (load balancing)</li>
    <li>Map-Reduce Support</li>
    <li>GridFS</li>
</ul>
<br>
<ul>Application of MongoDB
    <li>Content Management Systems</li>
    <li>Blogging Platforms</li>
    <li>Web Analytics</li>
    <li>E-Commerce</li>
    <li>Event Logging</li>
    <li>Systems where the type of data that needs to be stored can change dynamically.</li>    
</ul>
<br>
<ul>When NOT to use Document Stores
    <li>When you need support for complex transactions that operate on multiple documents</li>
    <li>When you data model is well-known and not expected to change</li>
</ul>
<br>