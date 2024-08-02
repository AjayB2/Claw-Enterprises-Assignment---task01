# My To-Do App

## API Endpoints

### Authentication

- **POST /api/auth/register**
    - Request: `{ "username": "test", "password": "password" }`
    - Response: `200 OK`

- **POST /api/auth/login**
    - Request: `{ "username": "test", "password": "password" }`
    - Response: `{ "auth": true, "token": "JWT_TOKEN" }`

### To-Dos

- **POST /api/todos**
    - Request: `{ "description": "Test todo", "status": "pending" }`
    - Response: `{ "id": 1 }`

- **GET /api/todos**
    - Response: `[{ "id": 1, "description": "Test todo", "status": "pending" }]`

- **PUT /api/todos/:id**
    - Request: `{ "description": "Updated todo", "status": "completed" }`
    - Response: `200 OK`

- **DELETE /api/todos/:id**
    - Response: `200 OK`

## Deployment

### Backend

1. Deploy the backend to Heroku.
2. Ensure the following environment variables are set:
    - `PORT`
    - `SECRET_KEY`

### Frontend

1. Deploy the frontend to Netlify or Vercel.
2. Configure the frontend to use the backend API URL.

