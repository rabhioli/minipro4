# Taskify  

+   Rabhi Alqadi


+ **Description:** Taskify is a user-friendly task management app that helps you stay organized and focused. Create, organize, and prioritize tasks effortlessly, ensuring nothing falls through the cracks. Stay productive and achieve more with Taskify.

+ Github Frontend:https://github.com/rabhioli/minipro4FE
+ Deployed:https://gilded-salmiakki-13dc05.netlify.app/


# List of Dependencies
+ Django
+ Django REST Framework
+ Environ
+ Cors-headers
+ PIP
+ Gunicorn
## ERD
User
- id: int (PK)
- username: string
- email: string
- password: string
- created_at: datetime
- updated_at: datetime

Task
- id: int (PK)
- title: string
- description: text
- due_date: datetime
- is_completed: boolean
- user_id: int (FK to User)


## Route Map:
| Route Name    | Endpoint               | Method | Description                               |
|---------------|------------------------|--------|-------------------------------------------|
| Task List     | /api/tasks/            | GET    | Retrieve all tasks                        |
| Create Task   | /api/tasks/            | POST   | Create a new task                         |
| Task Detail   | /api/tasks/:i  | GET    | Retrieve details of a specific task       |
| Update Task   | /api/tasks/:id   | PUT    | Update details of a specific task         |
| Delete Task   | /api/tasks/:id   | DELETE | Delete a specific task                    |
| User Signup   | /api/auth/signup/      | POST   | Create a new user account                 |
| User Login    | /api/auth/login/       | POST   | Authenticate user login                   |
| User Logout   | /api/auth/logout/      | POST   | Logout user                               |
| User Profile  | /api/users/profile/    | GET    | Retrieve user profile information         |
| Update Profile| /api/users/profile/    | PUT    | Update user profile information           |

## Mockup
![Desktop View](https://i.imgur.com/DtJyl50.png)
