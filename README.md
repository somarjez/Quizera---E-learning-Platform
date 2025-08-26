# QUIZERA: An E-Learning Platform

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Django](https://img.shields.io/badge/Django-4.0+-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Status-In%20Development-orange.svg)

## 📚 Overview

QUIZERA is a comprehensive Python-based e-learning platform designed specifically for computer science students. The platform combines structured learning with gamified quizzes, formal assessments, and digital certification to create an engaging educational experience.

## 🎯 Objectives

### General Objective
To develop a Python-based Student E-Learning Platform that provides structured lessons, interactive quizzes, formal exams, and certificates of completion.

### Specific Objectives
1. **User-Friendly Design**: Create an intuitive platform where computer science students can easily enroll and study
2. **Interactive Quizzes**: Implement game-like quizzes with time limits, instant feedback, and scoring systems
3. **Assessment Module**: Develop comprehensive exams that evaluate overall course knowledge
4. **Digital Certification**: Generate PDF certificates for successful course completion
5. **Admin Management**: Enable administrators to create and manage courses, lessons, quizzes, and exams
6. **Progress Tracking**: Monitor student progress with completion percentages and performance analytics

## ✨ Key Features

### For Students
- 📖 **Course Enrollment**: Browse and enroll in available courses
- 🎮 **Interactive Quizzes**: Gamified learning experience with:
  - Time-limited questions
  - Instant feedback
  - Score tracking
  - Progress indicators
- 📝 **Formal Exams**: Comprehensive assessments for course completion
- 🏆 **Digital Certificates**: Auto-generated PDF certificates upon successful completion
- 📊 **Progress Dashboard**: Track learning progress and performance metrics

### For Administrators
- 📚 **Course Management**: Create, edit, and organize courses
- 📄 **Lesson Creation**: Develop structured learning content
- ❓ **Quiz Builder**: Design interactive quizzes with multiple question types
- 📋 **Exam Management**: Create and schedule formal assessments
- 👥 **User Management**: Manage student accounts and enrollments
- 📈 **Analytics**: Monitor platform usage and student performance

## 🛠️ Technology Stack

- **Backend**: Python with Django/Flask framework
- **Database**: SQLite (development) / MySQL (production) / Firebase (cloud option)
- **Frontend**: HTML5, CSS3, JavaScript
- **PDF Generation**: ReportLab or WeasyPrint
- **Authentication**: Django Auth or Flask-Login
- **Deployment**: Compatible with Heroku, AWS, or similar platforms

## 📋 System Requirements

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)
- Virtual environment (recommended)
- Modern web browser

### Dependencies
```
Django>=4.0.0
Pillow>=9.0.0
reportlab>=3.6.0
python-decouple>=3.6
django-crispy-forms>=1.14.0
```

## 🚀 Installation Guide

### 1. Clone the Repository
```bash
git clone https://github.com/jramo/quizera.git
cd quizera
```

### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Database Setup
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create Superuser
```bash
python manage.py createsuperuser
```

### 6. Run Development Server
```bash
python manage.py runserver
```

Access the platform at `http://localhost:8000`

## 📁 Project Structure

```
quizera/
├── quizera/                 # Main project directory
│   ├── settings.py         # Django settings
│   ├── urls.py            # URL routing
│   └── wsgi.py            # WSGI configuration
├── apps/
│   ├── accounts/          # User authentication
│   ├── courses/           # Course management
│   ├── quizzes/          # Quiz functionality
│   ├── exams/            # Exam system
│   ├── certificates/     # Certificate generation
│   └── dashboard/        # User dashboards
├── static/               # Static files (CSS, JS, images)
├── templates/            # HTML templates
├── media/               # User-uploaded files
├── requirements.txt     # Python dependencies
└── manage.py           # Django management script
```

## 🎮 Usage Guide

### For Students
1. **Registration**: Create an account using email and password
2. **Browse Courses**: Explore available computer science courses
3. **Enroll**: Join courses of interest
4. **Study**: Access lessons and learning materials
5. **Take Quizzes**: Complete interactive quizzes for each lesson
6. **Attempt Exams**: Take final exams when ready
7. **Download Certificates**: Get PDF certificates upon successful completion

### For Administrators
1. **Login**: Access admin panel with superuser credentials
2. **Create Courses**: Add new courses with descriptions and objectives
3. **Add Lessons**: Create structured learning content
4. **Build Quizzes**: Design interactive assessments
5. **Manage Users**: Monitor student progress and enrollments
6. **Generate Reports**: View platform analytics and performance metrics

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the project root:

```env
SECRET_KEY=your-secret-key-here
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_HOST_USER=your-email@gmail.com
EMAIL_HOST_PASSWORD=your-app-password
```

### Database Configuration
The platform supports multiple database backends:
- **SQLite**: Default for development
- **MySQL**: Recommended for production
- **Firebase**: For cloud-based deployment

## 📊 Features in Detail

### Interactive Quiz System
- Multiple choice questions
- True/false questions
- Fill-in-the-blank
- Time limits per question
- Immediate feedback
- Score calculation
- Progress tracking

### Exam Module
- Comprehensive assessments
- Randomized question order
- Time limits
- Auto-submission
- Detailed results
- Pass/fail determination

### Certificate Generation
- Automatic PDF creation
- Personalized with student name
- Course completion details
- Digital signatures
- Download and email options

## 🔒 Security Features

- User authentication and authorization
- CSRF protection
- SQL injection prevention
- XSS protection
- Secure password handling
- Session management

## 📈 Future Enhancements

- Mobile application development
- Multiplayer quiz competitions
- External teacher content uploads
- Video lesson integration
- Discussion forums
- Advanced analytics dashboard
- Integration with external LMS
- AI-powered content recommendations

## ⚠️ Limitations

- **Single-player quizzes only**: No multiplayer competitions in current version
- **Auto-generated certificates**: Not formally accredited by external institutions
- **Admin-only content**: No external teacher uploads
- **Web-only access**: No mobile app in this version
- **Limited multimedia**: Basic support for images and text

## 🤝 Contributing

We welcome contributions to QUIZERA! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Team

- **Project Lead**: Jezreel Ramos
- **Backend Developer**: Jezreel Ramos, Judeelyn Capili
- **Frontend Developer**: Shaila Avellaneda, Shaine Macatangay
- **UI/UX Designer**: Team Quizera



## 🏆 Acknowledgments

- Django community for the excellent framework
- Open source contributors
- Computer science education community
- Beta testers and early adopters

---

**Built with ❤️ for Computer Science Education**