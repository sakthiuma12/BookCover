# Experiment 05: Book Back-Cover Page Design

**Date:** ____________________

## Aim

To design a book back-cover page using HTML and CSS and serve it locally with Django.

## Software requirements

- Python 3.10 or later
- Django 5.2
- A modern web browser

## Design steps

1. Create a Django project named `bookcover_project`.
2. Create the `cover_page` application and add it to `INSTALLED_APPS`.
3. Add a Django view and URL route for the home page.
4. Create `templates/cover_page/` for the HTML template and
   `static/cover_page/` for the stylesheet and image.
5. Write the book-cover content in HTML and its layout and colors in CSS.
6. Add the locally stored SVG illustration to the cover.
7. Start Django's development server and open the page on localhost.

## Project structure

```text
book_cover/
├── bookcover_project/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
├── cover_page/
│   ├── templates/cover_page/index.html
│   ├── static/cover_page/css/style.css
│   ├── static/cover_page/images/night-sky.svg
│   ├── urls.py
│   └── views.py
├── manage.py
└── requirements.txt
```

## Program

The complete program is in this project. The Django view renders
`cover_page/templates/cover_page/index.html`; Django's static files serve the
stylesheet and SVG illustration from `cover_page/static/`.

The design contains a title and tagline, book synopsis, review quotation,
author details, publisher mark, and decorative barcode. Its layout adapts to
mobile screens.

## Run the program

From the project directory, create and activate a virtual environment, then
install the dependency:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

Start the development server:

```powershell
python manage.py runserver
```

Open <http://127.0.0.1:8000/> in a browser to view the cover. The Django admin
is available at <http://127.0.0.1:8000/admin/>. To create an admin login, run
`python manage.py createsuperuser` in a separate terminal after installing
Django.

## Output

A responsive, dark green and gold book back-cover design with original
moonlit-valley artwork, readable book description, review quote, author and
publisher information, and a decorative barcode.

## Result

The program for designing a book back-cover page using HTML, CSS, and Django
was completed successfully.
