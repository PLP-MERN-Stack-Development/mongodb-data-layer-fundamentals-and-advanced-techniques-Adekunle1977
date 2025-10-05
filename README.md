📚 PLP MERN Stack Development - Week 1: MongoDB Assignment
This repository contains the solution files for the MongoDB Data Layer Fundamentals and Advanced Techniques assignment.

🚀 Objective
This assignment demonstrates fundamental and advanced MongoDB operations, including database setup, CRUD operations, advanced queries, aggregation pipelines, and indexing.

📁 Repository Contents
File	Purpose
insert_books.js	The script used to set up the initial database by inserting a minimum of 10 book documents.
queries.js	Contains all the MongoDB shell queries (db.collection.find(), db.collection.aggregate(), etc.) for Tasks 2, 3, 4, and 5.
README.md	This setup guide and explanation.
[Your Screenshot Name]	A screenshot showing the plp_bookstore database and books collection in MongoDB Compass/Atlas.
🛠️ Setup and Execution Instructions
Follow these steps to replicate the assignment environment and run the solution scripts.

Prerequisites
MongoDB Installation: MongoDB Community Edition (or access to a free MongoDB Atlas cluster).

MongoDB Shell (mongosh): Used to interact with the database and run the scripts.

Step 1: Initialize the Database and Collection
Open your terminal or command prompt.

Start the MongoDB Shell (mongosh) and connect to your local or Atlas instance.

Execute the insert_books.js script to create the plp_bookstore database, the books collection, and insert the initial data:

Bash

# Run this command in your regular terminal, NOT inside the mongosh shell
mongosh <URI_or_connection_string> --file insert_books.js
(If using a local MongoDB instance, you can typically omit the URI: mongosh --file insert_books.js)

Step 2: Execute Queries and Advanced Tasks
Start the MongoDB Shell (mongosh) and connect to your database.

Switch to the correct database:

JavaScript

use plp_bookstore
The file queries.js contains all the necessary commands for Tasks 2, 3, 4, and 5. To execute and verify these queries, you can either:

Method A (Preferred): Paste the contents of queries.js directly into the mongosh shell.

Method B: Run the entire script as a file (though sometimes aggregation outputs can be messy this way):

Bash

# Run this command in your regular terminal
mongosh <URI_or_connection_string> --file queries.js
✅ Performance Demonstration (Task 5: Indexing)
The following lines in queries.js were used to demonstrate the index performance using the explain() method:

[Copy/Paste the query you used for the title index here]

[Copy/Paste the query you used for the author and published_year compound index here]
