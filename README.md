Create a CRUD API for a simple Course Library application. The API can be used to create authors and courses. Authors will have first name, last name, DOB, email id properties. An author can write one or more courses. Each course should have a title and description.
Via a REST API it must be possible to:

List all authors
Add a new author
Create courses for an author
List all courses for an author
Get one course for an author by the course identifier
Update course for an author
Partially update course for an author using patch request
Delete course for an author
Create a batch of authors using a single endpoint
Get a batch of authors corresponding to multiple author identifiers passed as parameter to an endpoint
Implement paging and sorting(by name for authors and by title for courses) for all endpoints that return multiple results
The author should receive an email with the course title everytime a course is added for him/her

User authentication is NOT required. The data doesn't need to be persisted, You can either use EF Core's in-memory database or a mock data repository that can hold data in a Dictionary/ConcurrentDictionary data structure. However, please ensure that the mock data repository methods are asyncronous.
This link gives an overview of adding test data and configuring in-memory database using EF Core: https://stormpath.com/blog/tutorial-entity-framework-core-in-memory-database-asp-net-core
Sending of the email can be mocked by simply printing the email id of the user in the console instead of using a SMTP server to send an actual email.
