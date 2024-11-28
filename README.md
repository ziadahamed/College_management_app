


College Management Application
This is a College Management Application designed for efficient handling of student and faculty information.

Technology Stack
Frontend: React
Backend: Django REST Framework
Database: PostgreSQL
Features
Login Page
The application starts with a login page where the user needs to:

Enter their email ID and password.
Choose their role: Student or Faculty.
Click the Login button to proceed to their respective dashboard.
Faculty Dashboard
After logging in as a faculty member, the Faculty Dashboard provides the following features:

View all students' details.
Add new students.
Assign subjects to students and link them to the appropriate faculty.
Edit student details.
Log out.
Student Dashboard
After logging in as a student, the Student Dashboard provides the following features:

Display a brief overview of the student’s details.
View and edit their own details.
View assigned subjects and the respective faculty.
Log out.
Backend Functionality
The backend is built using the Django REST Framework. It supports the following CRUD operations:

GET: Fetch user details.
POST: Add new entries.
PUT: Update existing records.
DELETE: Remove records.
Current Issue
There is an issue with connecting the Django backend to the PostgreSQL database. The database settings in the settings.py file are as follows:

python

DATABASES = { 
   'default': { 
        'ENGINE': 'django.db.backends.postgresql', 
        'NAME': 'University', 
        'USER': 'ziad', 
        'PASSWORD': 'ziad', 
        'HOST': 'localhost',  # or your PostgreSQL server's address 
        'PORT': '5432', 
   } 
}
Despite the configuration, an error occurs while connecting to the database.

Database Structure
The database is built in PostgreSQL with the following details:

Database Name: University
Tables:
Student
Subject
student_enrollment
faculty
user_management
All tables have been created successfully.
