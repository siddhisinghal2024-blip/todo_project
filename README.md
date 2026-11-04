Django To-Do List Web Application

A simple and user-friendly To-Do List Web Application built using Python and Django. This project helps users organize their daily activities by creating, managing, updating, and tracking tasks.

Features

* Add Tasks: Create new tasks with a title and description.
* View Tasks: Display all tasks in an organized table.
* Edit Tasks: Update existing task details.
* Delete Tasks: Remove tasks that are no longer required.
* Task Completion: Mark tasks as completed using a checkbox.
* Creation Date: Automatically store the date and time when a task is created.
* Database Integration: Store task information using SQLite.

 Technologies Used

* Python
* Django
* HTML
* CSS
* SQLite

 Project Structure

todo_project/
│
├── tasks/
│   ├── migrations/
│   ├── templates/
│   ├── static/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── admin.py
│
├── todo_project/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── db.sqlite3
├── manage.py
└── README.md

 Installation and Setup

Follow these steps to run the project locally.

1. Clone the Repository

git clone YOUR_GITHUB_REPOSITORY_URL

2. Navigate to the Project Folder

cd todo_project

3. Create a Virtual Environment

python3 -m venv myenv

4. Activate the Virtual Environment

For macOS/Linux:

source myenv/bin/activate

5. Install Django

pip install django

6. Apply Database Migrations

python manage.py migrate

7. Run the Development Server

python manage.py runserver

8. Open in Browser


 Project Objective

The main objective of this project is to understand Django web development concepts, including:

* Django project and app structure
* Models and database management
* Views and URL routing
* HTML templates
* CRUD operations (Create, Read, Update, Delete)
* SQLite database integration

Author

Siddhi Singhal

B.Sc. Business Analytics Student
