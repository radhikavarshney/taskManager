# Task Manager

A simple task manager application built with Node.js, Express, and MongoDB. This project allows users to create, read, update, and delete tasks.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [License](#license)

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/radhikavarshney/taskManager.git
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

3. Create a `.env` file in the root of the project and add your MongoDB URI:
    ```sh
    MONGO_URI=your_mongodb_uri
    JWT_LIFETIME = 5h
    ```

4. Start the server:
    ```sh
    npm start
    ```

## Usage

Once the server is running, you can access the application in your web browser at `http://localhost:3000`.

## API Endpoints

### Get All Tasks
- **URL:** `/api/v1/tasks`
- **Method:** `GET`
- **Description:** Retrieve all tasks.

### Get Single Task
- **URL:** `/api/v1/tasks/:id`
- **Method:** `GET`
- **Description:** Retrieve a single task by ID.

### Create Task
- **URL:** `/api/v1/tasks`
- **Method:** `POST`
- **Description:** Create a new task.
- **Body Parameters:**
  - `name`: (string) The name of the task.
  - `completed`: (boolean) The completion status of the task.

### Update Task
- **URL:** `/api/v1/tasks/:id`
- **Method:** `PATCH`
- **Description:** Update an existing task by ID.
- **Body Parameters:**
  - `name`: (string) The name of the task.
  - `completed`: (boolean) The completion status of the task.

### Delete Task
- **URL:** `/api/v1/tasks/:id`
- **Method:** `DELETE`
- **Description:** Delete a task by ID.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
