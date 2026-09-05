# Express.js API Planning

## Project Overview

This project focuses on planning the RESTful APIs required for a React.js To-Do List application.

The actual API implementation will be done in subsequent classes. This task focuses only on identifying and planning the required APIs.

---

## 1. Add Task

### API Endpoint

POST /api/tasks

### Purpose

Creates a new task in the To-Do List application.

### Request Body

{
  "title": "Complete React Assignment",
  "description": "Finish API planning task",
  "completed": false
}

### Response

{
  "id": 1,
  "title": "Complete React Assignment",
  "description": "Finish API planning task",
  "completed": false
}

---

## 2. Get All Tasks

### API Endpoint

GET /api/tasks

### Purpose

Retrieves all tasks from the To-Do List application.

### Response

[
  {
    "id": 1,
    "title": "Complete React Assignment",
    "description": "Finish API planning task",
    "completed": false
  },
  {
    "id": 2,
    "title": "Study JavaScript",
    "description": "Practice JavaScript concepts",
    "completed": true
  }
]

---

## 3. Get a Single Task

### API Endpoint

GET /api/tasks/:id

### Purpose

Retrieves a specific task using its unique ID.

### Example Request

GET /api/tasks/1

### Response

{
  "id": 1,
  "title": "Complete React Assignment",
  "description": "Finish API planning task",
  "completed": false
}

---

## 4. Update Task

### API Endpoint

PUT /api/tasks/:id

### Purpose

Updates an existing task.

### Example Request

PUT /api/tasks/1

### Request Body

{
  "title": "Complete Express Assignment",
  "description": "Complete the API planning work",
  "completed": true
}

### Response

{
  "id": 1,
  "title": "Complete Express Assignment",
  "description": "Complete the API planning work",
  "completed": true
}

---

## 5. Delete Task

### API Endpoint

DELETE /api/tasks/:id

### Purpose

Deletes a specific task using its unique ID.

### Example Request

DELETE /api/tasks/1

### Response

{
  "message": "Task deleted successfully"
}

---

## 6. Mark Task as Completed

### API Endpoint

PATCH /api/tasks/:id

### Purpose

Updates the completion status of a task.

### Example Request

PATCH /api/tasks/1

### Request Body

{
  "completed": true
}

### Response

{
  "id": 1,
  "title": "Complete React Assignment",
  "description": "Finish the API planning work",
  "completed": true
}

---

## RESTful API Summary

| Functionality | HTTP Method | Endpoint |
|---|---|---|
| Add Task | POST | /api/tasks |
| Get All Tasks | GET | /api/tasks |
| Get Single Task | GET | /api/tasks/:id |
| Update Task | PUT | /api/tasks/:id |
| Delete Task | DELETE | /api/tasks/:id |
| Mark Task Complete | PATCH | /api/tasks/:id |

---

## Task Data Structure

| Field | Type | Description |
|---|---|---|
| id | Number | Unique identifier of the task |
| title | String | Title of the task |
| description | String | Details about the task |
| completed | Boolean | Shows whether the task is completed |

---

## HTTP Status Codes

| Status Code | Meaning |
|---|---|
| 200 | Request successful |
| 201 | Task created successfully |
| 400 | Bad request |
| 404 | Task not found |
| 500 | Internal server error |

---

## RESTful Design Principles

The API follows RESTful design principles:

- Use HTTP methods according to the operation.
- Use meaningful resource-based URLs.
- Use unique IDs for tasks.
- Use JSON for request and response data.
- Use appropriate HTTP status codes.
- Keep API endpoints simple and predictable.

---

## Future Implementation

The actual APIs will be implemented in subsequent classes.

Possible technologies include:

- Node.js
- Express.js
- REST API
- JSON or Database
- React.js frontend

---

## Conclusion

This document defines the API requirements for the main functionalities of a React.js To-Do List application.

The current task focuses on API planning and does not include actual API implementation.

## Author
Disha kumawat