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
<h5>
<ul>What is MongoDB
  <li>Document Store</li>
  <li>Most popular document store, according to db-engines.com showing</li>
  <li>Designed for ease of development and scaling</li>
  <li>Supported by numerous programming languages</li>
  <li>Developed by 10gen in 2007</li>
</ul>
<br>
<ul>Main features of MongoDB
    <li>1. Ad-hoc queries.(namely "on the fly query",which is a query that cannot be determined prior to the moment the query is issued.<br> e.g. var queryStr="select * from table wherhe id="+myId . It is an entirely different query each time the line code is executed depending on the value of myId. The opposite of an Ad-hoc query <br>is a predefined query like Stored Procedure, where you have created a single query for the entire generalized<br> purpose of selecting fron that table and pass the ID as a variable.)</li>
    <li>2. Indexing and Secondary Indexing</li>
    <li>3. Replication</li>
    <li>4. Sharding (load balancing) {Sharding is a type of database partitioning that seperates very large database <br>into smaller,faster,more easily managed partes. In MongoDB, sharding is a method for distributing data across <br>multiple machines.MongoDB uses sharding to support deployments with very large data sets and <br>high throughput operations.}</li>
    <li>5. Map-Reduce Support</li>
    <li>6. GridFS (which is the MongoDB specification for storing and retrieving very large files such as images, audio files etc. <br>It is kind of a file system to store files but its data is stored within MongoDB collections.)</li>
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

Note: there are four types of NoSQL: 
Column family database(Cassandra,HBase,Bigtable), In column-oriented NoSQL database, data is stored in cells grouped in columns of data rather than as rows of data. Columns are logically grouped into column families.  In comparison, most relational DBMS store data in rows, the benefit of storing data in columns, is fast search/ access and data aggregation. Relational databases store a single row as a continuous disk entry. Different rows are stored in different places on disk while Columnar databases store all the cells corresponding to a column as a continuous disk entry thus makes the search/access faster. <br><br>
Document database(CouchDB,MongoDB), schema-less. One key difference between a key-value store and a document store is that the latter embeds attribute metadata associated with stored content, which essentially provides a way to query the data based on the contents. <br><br>
Key-value database(Dynamo,HBase,Redis,Bigtable), schema-less format of a key value database<br><br>
Graph database(Neo4, InfoGrid).
<br><br>Collumn DB example:<br>
{
3PillarNoida: {
city: Noida
pincode: 201301
},
details: {
strength: 250
projects: 20
}
}
{
3PillarCluj: {
address: {
city: Cluj
pincode: 400606
}, 
details: {
strength: 200
projects: 15
}
},
{
3PillarTimisoara: {
address: {
city: Timisoara
pincode: 300011
},
details: {
strength: 150
projects: 10
}
}
{
3PillarFairfax : {
address: {
city: Fairfax
pincode: VA 22033
}, 
details: {
strength: 100
projects: 5
}
}
<br>
The outermost keys 3PillarNoida, 3PillarCluj, 3PillarTimisoara and 3PillarFairfax are analogues to rows.
‘address’ and ‘details’ are called column families.<br>
The column-family ‘address’ has columns ‘city’ and ‘pincode’.<br>
The column-family details’ has columns ‘strength’ and ‘projects’.<br>
Columns can be referenced using CloumnFamily.
<br>
Google’s BigTable, HBase and Cassandra are the most popular column store based databases.
</h5>

