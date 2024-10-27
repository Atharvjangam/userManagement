##User Management Dashboard
This web application is a user management dashboard that allows users to create, update, and delete user records.

#Technologies Used
UI: Next.js, Tailwind CSS
Backend: Spring Boot, Java, REST

#Features
Create, update, and delete users
Responsive and user-friendly interface
RESTful API for backend communication

#API Documentation
Four APIs are created to perform CRUD operations on the user list:

1. Get All Users
REST Method: GET
URL: http://localhost:8080/api/public/users
Request: None
Response:
    Returns a list of users in JSON format.
    Example Response:
    [
        {
            "userId": 1,
            "firstName": "Atharv",
            "lastName": "Jangam",
            "email": "xghz",
            "userName": "A1"
        },
        ...
    ]

2. Update a User
REST Method: PUT
URL: http://localhost:8080/api/public/users?userId=1
Request:
    {
        "firstName": "Ath",
        "lastName": "Jangam",
        "email": "xghz"
    }
Response:
Returns null on successful update.

3. Delete a User
REST Method: DELETE
URL: http://localhost:8080/api/public/users?userId=1
Request: User ID as a path parameter.
Response:
Returns null on successful deletion.

4. Create a User
REST Method: POST
URL: http://localhost:8080/api/public/createUser
Request:
    {
        "firstName": "Atharv",
        "lastName": "Jangam",
        "email": "xghz",
        "userName": "A1"
    }
Response:
Returns null on successful creation.


##Getting Started
Clone the Repository: https://github.com/Atharvjangam/userManagement/blob/main

bash
git clone <repository-url>

Backend Setup:

Navigate to the backend directory.
Run the Spring Boot application:
bash
./mvnw spring-boot:run


Frontend Setup:

Navigate to the frontend directory.
Install dependencies:
bash
npm install

Run the Next.js application:
bash
npm run dev


Open your browser and go to http://localhost:3000 for the frontend.
Access the API at http://localhost:8080/api/public/....
