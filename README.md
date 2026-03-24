# College Management Website (LITAM)

A full-stack college management system built with React.js and Django REST Framework.

## Features
- **Faculty Management**: Browse faculty profiles by department.
- **Course Catalog**: View available undergraduate and postgraduate programs.
- **Student Portal**: Access study materials, timetables, and results.
- **Notice Board**: Stay updated with the latest college announcements.
- **Gallery**: Visual tour of the campus.
- **Contact**: Reach out to the administration via a contact form.
- **Admin Dashboard**: Manage all content through the Django Admin interface.

## Technologies Used
- **Frontend**: React.js, React Router, Axios, Lucide-React, CSS3 (Responsive Design).
- **Backend**: Python Django, Django REST Framework, MySQL.
- **Communication**: REST APIs with CORS enabled.

---

## Setup Instructions

### Backend Setup (Django)
1. **Navigate to the backend folder**:
   ```bash
   cd backend
   ```
2. **Create a virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies**:
   ```bash
   pip install django djangorestframework django-cors-headers mysqlclient Pillow
   ```
4. **Configure Database**:
   - Create a MySQL database named `college_db`.
   - Update `DATABASES` settings in `core/settings.py` with your MySQL credentials.
5. **Run Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
6. **Create a Superuser** (for Admin access):
   ```bash
   python manage.py createsuperuser
   ```
7. **Start the server**:
   ```bash
   python manage.py runserver
   ```

### Frontend Setup (React)
1. **Navigate to the frontend folder**:
   ```bash
   cd frontend
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Start the development server**:
   ```bash
   npm start
   ```

---

## API Endpoints
- `GET /api/faculty/` - List all faculty
- `GET /api/courses/` - List all courses
- `GET /api/notices/` - List all announcements
- `GET /api/gallery/` - List gallery images
- `GET /api/students/` - List student resources

## Future Enhancements
- JWT-based authentication for student login.
- Online fee payment integration.
- Attendance tracking system.
- Placement portal for students.
