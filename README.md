# CS50W Project 1: Wiki

This is a Django-based Wikipedia-style encyclopedia site built as part of the CS50 Web Programming with Python and JavaScript course.

## Core Features

- Index Page
- Entry Page
- Search
- New Page
- Edit Page
- Random Page
- Markdown Conversion 

## Technologies

- **Python** 3.10.x  
- **Django** 3.2.4 — Web framework used for backend logic and routing  
- **markdown2** — Library to convert Markdown content into HTML  
- **setuptools** >= 65.0 — Build tool to ensure compatibility with legacy `distutils` packages  
- **django-debug-toolbar** — In-browser debug panel for inspecting Django apps


## Requirements

Install required packages with:

```bash
pip install -r requirements.txt
```

Dependencies include:
- Django==3.2.4
- markdown2
- setuptools >= 65.0
- django-debug-toolbar==4.3.0

Make sure all these packages are installed to avoid errors during migration or development.

## Getting Started

1. **Clone this repository**:

    ```bash
    git clone https://github.com/me50/HankChoose.git
    cd HankChoose
    git checkout web50/projects/2020/x/wiki
    ```

2. **Create a virtual environment**:

    ```bash
    python3.10 -m venv .venv
    source .venv/bin/activate.ps1 # on Linux/macOS   
    .venv\Scripts\activate.bat    # On Windows 
    ```

3. **Install dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Run database migrations**:

    ```bash
    python manage.py migrate
    ```
5. **(Optional) Create a superuser to access Django admin site**:

    ```bash
    python manage.py createsuperuser 
    ```
    then visit http://127.0.0.1:8000/admin
6. **Run the development server**:

    ```bash
    python manage.py runserver
    ```

7. **Open the site**:

    Open your browser and go to:  
    http://127.0.0.1:8000

## Project Structure

```
wiki/
├── manage.py
├── encyclopedia/        # Django app (views, URLs, templates)
├── wiki/                # Project settings (settings.py, urls.py)
├── entries/             # Markdown entry files
├── requirements.txt
├── .gitignore
└── README.md  
```

## Notes

- All encyclopedia entries are stored as Markdown files in the `entries/` folder.  
- Do not commit `db.sqlite3`, virtual environments, or other unnecessary files.  
- Include `.gitignore` and `requirements.txt` in your submission.  

## Author

Haiyin Chen (English name: Hank Chen) – hankchenv@gmail.com

## License

This project is part of the CS50W coursework and is provided for educational purposes only.
