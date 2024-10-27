# Email Sender Using Django

This project demonstrates how to build a simple email sender using Django. It allows users to send emails through a web interface by filling out necessary fields like the recipient's email, subject, and message content.

## Table of Contents
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
- [Project Structure](#project-structure)
- [Usage](#usage)

---

## Requirements
- Python 3.x
- Django 3.x or later

## Setup Instructions
1. **Clone the Repository**
   ```bash
   git clone https://github.com/pavithrak17/Email-Sender-Using-Django.git
   cd your projectname
   ```

2. **Create and Activate a Virtual Environment**
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**
   - Update your email credentials in the `settings.py` file or create a `.env` file to securely store them.
   - Example:
     ```python
     EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
     EMAIL_HOST = 'smtp.example.com'
     EMAIL_PORT = 587
     EMAIL_USE_TLS = True
     EMAIL_HOST_USER = 'your-email@example.com'
     EMAIL_HOST_PASSWORD = 'your-email-password'
     ```

5. **Run Migrations**
   ```bash
   python manage.py migrate
   ```

6. **Run the Django Development Server**
   ```bash
   python manage.py runserver
   ```

## Project Structure
- **views.py** - Contains logic for handling email form submissions and sending emails.
- **urls.py** - Routes the project URLs to the appropriate views.
- **templates/home.html** - The frontend interface where users can input email details.

## Usage
1. Open the application in your browser: [http://127.0.0.1:8000](http://127.0.0.1:8000).
2. Fill in the recipient's email, subject, and message.
3. Click "Send Email" to send the email.

---
```
If You like the project, click on ⭐!
```
