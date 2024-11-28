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
Database Plan
I initially planned the database and tables to manage data efficiently. Here’s the structure and functionality I envisioned:

Tables:

Student: Stores student information.
Subject: Maintains a list of subjects offered.
student_enrollment: Links students to subjects and their faculty.
faculty: Contains faculty details.
user_management: Manages user login and roles.
Functionality:

The data stored in these tables would be displayed in the UI.
Users could perform CRUD operations via the UI, such as:
Save new data into the database (e.g., adding a new student or subject).
View all data dynamically on the frontend.
Subject and faculty assignments would also be handled and saved in the database for viewing and editing.
Current Issue
Due to a backend error, I couldn’t fully implement this plan. The issue lies in connecting the Django application to the PostgreSQL database. The database settings in the settings.py file are as follows:

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
Despite configuring the database, the connection isn’t working as expected.

Database Details
The database is built in PostgreSQL with the following details:

Database Name: University
Tables:
Student
Subject
student_enrollment
faculty
user_management
The tables have been created successfully, but the data couldn’t be integrated fully due to the backend issue mentioned above.

Status
The project is almost complete, with most functionalities implemented. The pending issues are:

Fixing the database connection error.
Conducting thorough testing to ensure smooth operation.
