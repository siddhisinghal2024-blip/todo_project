# My To-Do List – Django Web Application

## 1. Project Overview

My To-Do List is a simple task management web application developed using Python and Django. It helps users organize their daily activities by creating, viewing, editing, deleting, and marking tasks as completed.

The application uses Django for backend functionality, HTML and CSS for the user interface, and SQLite for storing task information.

## 2. Features

The application provides the following features:

1. **Add Tasks:** Users can create new tasks by entering a title and description.
2. **View Tasks:** All tasks are displayed in a structured table.
3. **Edit Tasks:** Users can modify the title and description of existing tasks.
4. **Delete Tasks:** Users can remove tasks that are no longer required.
5. **Mark as Completed:** A checkbox allows users to mark tasks as completed or pending.
6. **Task Status:** The completion status is stored in the database.
7. **Creation Date:** The application displays the date and time when each task was created.
8. **Database Integration:** All task details are stored using Django's SQLite database.

## 3. Technologies Used

- Python
- Django
- HTML
- CSS
- SQLite Database

## 4. Project Structure

The project is organized into the following folders and files:

```text
todo_project/
│
├── tasks/
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── templates/
│   ├── add.html
│   ├── edit.html
│   ├── home.html
│   └── index.html
│
├── static/
│   └── style.css
│
├── todo_project/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── db.sqlite3
├── manage.py
└── README.md
```

## 5. Database Model

The application uses a Django model named `Task` to store task information.

The model contains the following fields:

| Field | Description |
|---|---|
| id | Unique ID assigned to each task |
| title | Stores the task title |
| description | Stores the task description |
| completed | Stores the completion status (True/False) |
| created_at | Stores the task creation date and time |

### Completion Status

The `completed` field is a Boolean field.

- `0` – False (Task Pending)
- `1` – True (Task Completed)

Whenever a user ticks or unticks the checkbox, the completion status is updated in the SQLite database.

## 6. Installation and Setup

Follow these steps to set up and run the project on your computer.

### Step 1: Install Python

Download and install Python from:

https://www.python.org/downloads/

Check whether Python is installed:

```bash
python3 --version
```

### Step 2: Open the Project in VS Code

Open Visual Studio Code and open the project folder.

Open the terminal:

**Terminal → New Terminal**

Make sure the terminal is inside the folder containing `manage.py`.

### Step 3: Create a Virtual Environment

Run:

```bash
python3 -m venv myenv
```

### Step 4: Activate the Virtual Environment

```bash
source myenv/bin/activate
```


### Step 5: Install Django

Run:

```bash
pip install django
```

Check the Django version:

```bash
python -m django --version
```

### Step 6: Apply Database Migrations

Run:

```bash
python manage.py makemigrations
```

Then:

```bash
python manage.py migrate
```

These commands create and update the database tables required by the application.


### Step 7: Run the Django Development Server

Run:

```bash
python manage.py runserver
```
The To-Do List application will now be available.

## 7. How to Use the Application

1. Open the home page.
2. Click on the **Add Task** button.
3. Enter the task title and description.
4. Save the task to add it to the list.
5. View all saved tasks on the home page.
6. Click **Edit** to modify an existing task.
7. Tick the checkbox to mark a task as completed.
8. Untick the checkbox to mark it as pending.
9. Click **Delete** to remove a task.

## 8. Database Management

The application uses SQLite as its database.

The database file is named:

```text
db.sqlite3
```

It stores all task records, including their titles, descriptions, completion status, and creation dates.

The database can be inspected using an SQLite database viewer or the SQLite extension in Visual Studio Code.

## 9. GitHub Setup

To upload the project to GitHub:

### Step 1: Initialize Git

```bash
git init
```

### Step 2: Add Project Files

```bash
git add .
```

### Step 3: Commit Changes

```bash
git commit -m "Initial commit - Django To-Do List"
```

### Step 4: Connect Your GitHub Repository

Create a new repository on GitHub and connect it:

```bash
git remote add origin YOUR_GITHUB_REPOSITORY_URL
```

### Step 5: Push the Project

```bash
git branch -M main
git push -u origin main
```


## 10. Learning Outcomes

Through this project, the following Django concepts and practical skills are implemented:

- Understanding Django project and app structure.
- Creating Django models.
- Working with SQLite databases.
- Implementing Function-Based Views.
- Configuring URL routing.
- Using Django templates.
- Handling HTML forms and POST requests.
- Implementing CSRF protection.
- Performing CRUD operations.
- Updating Boolean fields through checkboxes.
- Using Git and GitHub for version control.
---

**Project:** My To-Do List  
**Purpose:** Task Management and Django Learning Project
