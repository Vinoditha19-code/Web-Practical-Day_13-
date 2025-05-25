# Web-Practical-Day_13-

01. index.js: 
It listens on port 3001 and handles JSON requests.
It uses a separate route (courseRoute) for managing course-related data.
It connects to a database called studentinfDB and logs whether the connection is successful or not.
Finally, it starts the server and prints a message confirming it's running.

02. Course.js
It creates a courseSchema with fields: code, name, credits, and description.
It then defines a Mongoose model named Course, linked to the "courses" collection.
A new course instance (webservice) is created with details about a Web Services course.
The course instance is saved to the database using .save().
Finally, the Course

03. CourseRoute
GET /: Retrieves all courses from the database and returns them in JSON format. If no data is found, it sends a "No data found" message.
GET /:id: Retrieves a specific course by its ID. If found, it sends the course data; otherwise, a "No data found" message.
GET /code/:cid: Attempts to find courses by their code, but there’s a small issue—the route is missing a leading /, so it won’t work correctly. 


![Screenshot 2025-05-25 150214](https://github.com/user-attachments/assets/444943e7-c59a-4056-a635-0a132983110f)
![Screenshot 2025-05-25 150124](https://github.com/user-attachments/assets/716643b8-efbe-4200-9561-334129619304)
