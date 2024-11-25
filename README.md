
---

# Project: Multi-Application Zango Project

This project contains three Zango applications developed as part of a multi-functional system:

1. **FirstApp**: A simple To-Do list management application.
2. **SecondApp**: A hospital management system for handling patient data.
3. **ThirdApp**: A student management system for maintaining student records.



## Project Structure

```
project/
│
├── workspaces/
│   ├── FirstApp/
│   │   ├── templates/
│   │   │   ├── todo_list.html
│   │   │   ├── add_todo.html
│   │   │   ├── edit_todo.html
│   │   │   └── delete_todo.html
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   ├── urls.py
│   │   └── forms.py
│   │
│   ├── SecondApp/
│   │   ├── templates/
│   │   │   ├── patient_list.html
│   │   │   ├── add_patient.html
│   │   │   ├── edit_patient.html
│   │   │   └── delete_patient.html
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   ├── urls.py
│   │   └── forms.py
│   │
│   ├── ThirdApp/
│   │   ├── templates/
│   │   │   ├── student_list.html
│   │   │   ├── add_student.html
│   │   │   ├── edit_student.html
│   │   │   └── delete_student.html
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   ├── urls.py
│   │   └── forms.py
│
├── my_test_urls.py
├── settings.py
└── db.sqlite3
```

---

## Applications

### **1. FirstApp - TASK List Manager**

**Features:**
- Create, view, update, and delete tasks.
- RESTful API integration for task management.
- Simple and intuitive interface for managing tasks.

**Endpoints:**
- `/api/todos/`: List all tasks.
- `/api/todos/add/`: Add a new task.
- `/api/todos/<id>/edit/`: Edit a task.
- `/api/todos/<id>/delete/`: Delete a task.

---

### **2. SecondApp - Hospital Management System**

**Features:**
- Manage patient data including name, age, contact details, and medical history.
- RESTful API integration for patient data operations.
- User-friendly interface for adding, editing, and deleting patient records.

**Endpoints:**
- `/api/patients/`: List all patients.
- `/api/patients/add/`: Add a new patient.
- `/api/patients/<id>/edit/`: Edit patient details.
- `/api/patients/<id>/delete/`: Delete patient data.

---

### **3. ThirdApp - Student Management System**

**Features:**
- Handle student data including first name, last name, gender, email, and enrollment date.
- RESTful API integration for student management.
- Modern interface for adding, editing, and deleting student records.

**Endpoints:**
- `/api/students/`: List all students.
- `/api/students/add/`: Add a new student.
- `/api/students/<id>/edit/`: Edit student details.
- `/api/students/<id>/delete/`: Delete student data.

---

## Setup Instructions

1. **Clone the Repository:**
   ```
   git clone <repository_url>
   cd project
   ```

2. **Install Dependencies:**
   ```
   pip install -r requirements.txt
   ```

3. **Setup the Database:**
   Create the tables for each application directly in the database or using SQL commands provided in the documentation.

4. **Run the Development Server:**
   ```
   python manage.py runserver
   ```

5. **Access Applications:**
   - FirstApp: `/api/todos/`
   - SecondApp: `/api/patients/`
   - ThirdApp: `/api/students/`

