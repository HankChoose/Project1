# CS50W Project 1: Wiki

This is a Django-based Wikipedia-style encyclopedia site built as part of the CS50 Web Programming with Python and JavaScript course.

## Features

- Create new encyclopedia entries  
- Edit existing entries  
- View individual entry pages  
- Search for entries (exact and partial matches)  
- Display a random entry  
- Use Markdown for content formatting  
- Error handling for duplicate entries and missing pages  

## Technologies

- **Python** 3.10.x  
- **Django** 3.2.4 — Web framework used for backend logic and routing  
- **markdown2** — Converts Markdown content into HTML  
- **setuptools** >= 65.0 — Ensures compatibility for legacy `distutils` dependencies

## Requirements

Install required packages with:

```bash
pip install -r requirements.txt
```

Dependencies include:
- Django==3.2.4
- markdown2

For local development and submission, only Django and markdown2 are required.

## Getting Started

1. **Clone this repository**:

    ```bash
    git clone https://github.com/me50/HankChoose.git
    cd HankChoose
    git checkout web50/projects/2020/1/wiki
    ```

2. **Create a virtual environment**:

    ```bash
    python3.10 -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    ```

3. **Install dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Run database migrations**:

    ```bash
    python manage.py migrate
    ```

5. **Run the development server**:

    ```bash
    python manage.py runserver
    ```

6. **Open the site**:

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
