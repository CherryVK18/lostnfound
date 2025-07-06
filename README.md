
# 🧳 Lost & Found Campus Platform

[![Live Site](https://img.shields.io/badge/Live%20Site-Visit%20Now-brightgreen?style=for-the-badge&logo=python)](https://tscharan.pythonanywhere.com)
[![Django](https://img.shields.io/badge/Django-4.2-092E20?style=for-the-badge&logo=django)](https://www.djangoproject.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.3-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)

A full-stack web application that helps students and staff report, search, and manage lost and found items across campus.

---

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| 🔐 **User Authentication** | Secure signup/login with profile management |
| 📍 **Map-Based Search** | Interactive map with geolocation for items |
| 📸 **Media Uploads** | Image uploads for better identification |
| 🔍 **Smart Filters** | Filter by keywords |
| 📱 **Mobile-Friendly** | Responsive design for all devices |

---

## 🛠️ Tech Stack

**Backend:**
- Django 4.2
- Python 3.10
- SQLite

**Frontend:**
- Tailwind CSS
- HTML5
- JavaScript (Vanilla)

**Deployment:**
- PythonAnywhere
- WhiteNoise (Static files)

---

## 🚀 Quick Start

### Local Development

1. **Clone the repo**
   ```bash
   git clone https://github.com/CherryVK18/lostnfound.git
   cd lostfound
   ```

2. **Set up virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate    # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment**
   ```bash
   cp .env.example .env
   # Edit .env with your settings
   ```

5. **Run migrations**
   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```

6. **Start development server**
   ```bash
   python manage.py runserver
   ```

Visit `http://localhost:8000`

---

## 📂 Project Structure

```bash
lostfound/
├── items/            # Item models and views
├── users/            # Authentication system
├── main/             # Core pages
├── static/           # CSS, JS, images
├── templates/        # HTML templates
├── lostfound/        # Project settings
└── manage.py         # Django CLI
```

---

## 🌐 Deployment

### PythonAnywhere Setup

1. Upload your code via Git or file manager
2. Create virtual environment:
   ```bash
   mkvirtualenv lostnfound --python=python3.10
   pip install -r requirements.txt
   ```
3. Configure WSGI file:
   ```python
   import os
   import sys
   path = '/home/yourusername/path/to/lostfound'
   if path not in sys.path:
       sys.path.append(path)
   os.environ['DJANGO_SETTINGS_MODULE'] = 'lostfound.settings'
   from django.core.wsgi import get_wsgi_application
   application = get_wsgi_application()
   ```
4. Set up static files in the Web tab

---

## 📸 Screenshots

| Page | Screenshot |
|------|------------|
| Homepage | ![Home](./ss/home.jpg) |
| Item Map | ![Map](./ss/map.jpg) |
| User Profile | ![Profile](./ss/profile.jpg) |

---

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---


## 👨‍💻 Author

**T. Sai Charan**  
[![GitHub](https://img.shields.io/badge/GitHub-CherryVK18-181717?style=flat&logo=github)](https://github.com/CherryVK18)

---

## 🙌 Acknowledgments

- Django Documentation
- PythonAnywhere Team
- Tailwind CSS Community
- All Beta Testers
