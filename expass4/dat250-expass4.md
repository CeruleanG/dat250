# Lab Report
## Technical problems
### Installation
no issue was encountered during the installation
### Connection failure
Issue: when the API was run, Postman cannot correctly connect to the database.
Cause: the default port in TodoAPI.java doesn't match the one in TodoAPITest.java
Solution: change the default port in TodoAPI.java to match the one in TodoAPITest.java
## Hard part
### To check if a `String` is numeric
Solution: using regex `"-?\\d+(\\.\\d+)?"`
### To retrieve properties when calling to PUT
Solution: using `req.body` to retrieve the Json String and translate it into a Java object using `gson.fromJson(req.body(),Todo.class)`
## Pending Issue
Experiment 3 and 4 are not done.
## Github link
https://github.com/CeruleanG/dat250-sparkjava-counter
