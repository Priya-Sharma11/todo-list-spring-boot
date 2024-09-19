# ToDo List Application

A simple ToDo list application built using **Spring Boot**. This application allows users to perform basic CRUD (Create, Read, Update, Delete) operations on tasks.

## Features

- Add new tasks
- Get a list of all tasks
- Get details of a specific task
- Update an existing task
- Delete a task

## Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- H2 Database (in-memory)
- Maven

## Prerequisites

To run this project, you need to have the following installed:

- [Java 8+](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Maven](https://maven.apache.org/)
- [Git](https://git-scm.com/)

## Setup Instructions

1. Clone the repository:
   git clone https://github.com/your-username/todo-list-spring-boot.git
   cd todo-list-spring-boot

2. Run the application:
   mvn spring-boot:run

3. Use Postman, or any other REST client to test the API endpoints.


## API Endpoints
The following endpoints are available for managing tasks in the ToDo List application:

1. Get all tasks
- Endpoint: /api/tasks
- Method: GET
- Description: Retrieves a list of all tasks.


2. Get task by ID
- Endpoint: /api/tasks/{id}
- Method: GET
- Description: Retrieves a task by its ID.
- Path Variable: id - The ID of the task.


3. Create a new task
- Endpoint: /api/tasks
- Method: POST
- Description: Creates a new task.


4. Update a task
- Endpoint: /api/tasks/{id}
- Method: PUT
- Description: Updates an existing task by ID.
- Path Variable: id - The ID of the task.


5. Delete a task
- Endpoint: /api/tasks/{id}
- Method: DELETE
- Description: Deletes a task by its ID.
- Path Variable: id - The ID of the task.

Open Postman.
1. Set the request method to GET.
- Enter the URL: http://localhost:8080/api/tasks.

2. Set the request method to GET.
- Enter the URL: http://localhost:8080/api/tasks/1 (replace 1 with the desired task ID).

3. Set the request method to POST.
- Enter the URL: http://localhost:8080/api/tasks.
- Select Body > raw > JSON and enter the task details:
- {
  "title": "New Task",
  "description": "Learn Spring Boot"
}

4. Set the request method to PUT.
- Enter the URL: http://localhost:8080/api/tasks/1 (replace 1 with the desired task ID).
- Select Body > raw > JSON and enter the updated task details:
- {
  "title": "Updated Task",
  "description": "Updated details"
}

5. Set the request method to DELETE.
- Enter the URL: http://localhost:8080/api/tasks/1 (replace 1 with the desired task ID).

Click Send.
