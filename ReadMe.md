# Add-question

simple application that allows users to add questions to a MySQL database using an HTML form.

Prerequisites: 
Before running the application, make sure you have the following software installed on your system:
1. Node.js
 
Navigate to present working directory and install the below using mentioned command in parenthesis

2. Express, mysql2, body parser (npm install express mysql2 body-parser)

Configuration: 

- Open the index.js file in the project directory.
- Modify the MySQL configuration section with your database credentials
  
Make sure you have created a table to store the questions
  
Query to create the table : 
  
CREATE TABLE questions (
    id INT AUTO_INCREMENT PRIMARY KEY,
    question TEXT NOT NULL,
    options JSON NOT NULL,
    correctOption INT NOT NULL
    );

Running : 

-run the app.js file (node app.js)

-You can now open your browser and visit http://localhost:3000

 
Usage : 
1. Fill in the question, options, and correct option in the form.
2. Click the "Submit" button to add the question to the MySQL database.
3. If the question is added successfully, you will see a success message. Otherwise, an error message will be displayed.


