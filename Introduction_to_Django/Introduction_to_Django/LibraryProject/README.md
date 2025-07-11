# 📚 Library Management System (Django)

A simple Django-based Library Management System designed to help users manage books, members, and borrowing activities efficiently. Built with Python and Django for a clean and maintainable backend structure.

---

## 🚀 Features

- 📖 Add, edit, and delete books
- 🔍 Search and filter books by title, author, or genre
- 👥 Register and manage members
- 📅 Track book borrowing and return dates
- 🔐 Admin panel for librarians
- 📊 Dashboard with basic statistics

---

## 🛠️ Tech Stack

- **Backend:** Python, Django
- **Frontend:** Django Templates (HTML, CSS, Bootstrap)
- **Database:** SQLite (default) or PostgreSQL/MySQL (optional)
- **Authentication:** Django's built-in auth system

---

## 📂 Project Structure

```
library_project/
│
├── library_project/          # Django project settings
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── library_app/              # Main library app
│   ├── migrations/
│   ├── templates/
│   ├── static/
│   ├── admin.py
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── forms.py
│
├── manage.py
├── db.sqlite3
├── README.md
└── requirements.txt
```

---

## 💻 Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/samya-abbas/Alx_DjangoLearnLab.git
cd library-project

# 2. Create and activate virtual environment
python -m venv myenv
source myenv/bin/activate  # On Windows: env\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run migrations
python manage.py migrate

# 5. Create a superuser for admin access
python manage.py createsuperuser

# 6. Start the development server
python manage.py runserver
```

Then open your browser and visit: [http://localhost:8000](http://localhost:8000)

---

## 📦 Core Django Models

- `Book`: Title, Author, ISBN, Genre, Copies Available
- `Member`: Name, Email, Contact Info
- `Borrowing`: Book, Member, Borrow Date, Return Date

---

## 🙌 Contributing

1. Fork the project
2. Create your feature branch: `git checkout -b feature/awesome-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/awesome-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## ✨ Acknowledgements

- Django Documentation (https://docs.djangoproject.com/)
- Open Source Community