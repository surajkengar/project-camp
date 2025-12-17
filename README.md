# Project Camp

## Overview
Project Camp is a web-based project and task management platform designed to help teams efficiently organize, track, and manage their projects and tasks, similar to Jira.

---

## Features
- User Authentication: Users can sign up and sign in to access the platform.
- Project Management: Users can create, update, and delete projects.
- Task Management: Users can add tasks, assign them to team members, update statuses, and track progress.
- Dashboard: Users can view project and task status through a dashboard.
- Admin Controls: Admin users can manage all projects, tasks, and user accounts.

---

## Technology Stack
- Frontend: React.js
- Backend: Node.js, Express
- Database: MongoDB (via Mongoose)
- Authentication: JSON Web Tokens (JWT)
- Environment Variables: dotenv for configuration

---

## API Endpoints
- User Authentication

- Sign Up: POST /api/user/signup

- Sign In: POST /api/user/signin

- Get Current User: GET /api/user/me (Requires JWT)

- Project Management

- Get All Projects: GET /api/project

- Add Project: POST /api/project (Admin only)

- Update Project: PUT /api/project/:projectId (Admin only)

- Delete Project: DELETE /api/project/:projectId (Admin only)

## Task Management

- Get All Tasks: GET /api/task

- Add Task: POST /api/task

- Update Task: PUT /api/task/:taskId

- Delete Task: DELETE /api/task/:taskId

## Middleware

- JWT authentication is used. Include a valid token in the Authorization header for protected routes.
