# 📝 Django Blog API Project

This is a Django-based Blog project with integrated Django REST Framework (DRF) for API development. It includes user account handling, blog management, and API routing, structured across modular Django apps.

---

## 🚀 Features

- Django-powered backend with modular app structure  
- RESTful APIs built using Django REST Framework  
- User account and blog post management  
- Well-organized project with clean architecture  
- Ready for deployment with static file handling

---

## 🗂️ Project Structure

```

blog/
├── accounts/         # Handles user accounts
│   ├── models.py
│   ├── serializers.py
│   ├── views.py, urls.py, etc.
│   └── migrations/
├── api/              # API routing app
│   └── urls.py
├── blog/             # Main project settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py, asgi.py
├── home/             # Blog content handling
│   ├── models.py
│   ├── serializers.py
│   ├── views.py, urls.py
│   └── migrations/
├── db.sqlite3        # SQLite database
├── manage.py         # Django management script
└── requirements.txt  # Python dependencies

````

---

## 🛠️ Installation

1️⃣ **Clone the repository:**
```bash
git clone https://github.com/your-username/blog.git
cd blog
````

2️⃣ **Create and activate virtual environment:**

```bash
python -m venv env
source env/bin/activate     # On Windows: env\Scripts\activate
```

3️⃣ **Install dependencies:**

```bash
pip install -r requirements.txt
```

4️⃣ **Apply migrations:**

```bash
python manage.py makemigrations
python manage.py migrate
```

5️⃣ **Run the development server:**

```bash
python manage.py runserver
```

---

## 📦 API Endpoints

Sample API base: `http://localhost:8000/api/`

| Method | Endpoint       | Description            |
| ------ | -------------- | ---------------------- |
| GET    | `/blogs/`      | List all blog posts    |
| POST   | `/blogs/`      | Create a new blog post |
| GET    | `/blogs/<id>/` | Retrieve a single post |
| PUT    | `/blogs/<id>/` | Update a post          |
| DELETE | `/blogs/<id>/` | Delete a post          |

*(Modify routes as per your `urls.py` setup.)*

---

## 🔧 Tech Stack

* **Python 3.x**
* **Django**
* **Django REST Framework**
* **SQLite** (default DB)
* **Bootstrap or custom CSS (optional)**

---

## ✍️ Author

**Dhananjay Pratap Singh**
Built with ❤️ using Django + DRF
