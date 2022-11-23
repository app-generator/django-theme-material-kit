# [Django Theme Material Kit](https://github.com/app-generator/django-theme-material-kit)

Modern template for **Django** coded on top of **Material Kit**, an open-source `Boostrap 5` design from `Creative-Tim`. 

> Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.

<br>

**Links & Resources**

- [Django Theme MKit](https://django-material-kit.appseed-srv1.com/) - LIVE Demo
- [Django Theme MKit](https://github.com/app-generator/django-theme-mkit-playground) - `playground project` 
- UI Kit: [Material Design BS5](https://www.creative-tim.com/product/material-kit?AFFILIATE=128200) `v3.0.3` by Creative-Tim

<br />

[![Django Theme Material Kit - Video Presentation.](https://user-images.githubusercontent.com/51070104/203492108-48d48000-2ad7-4dec-810a-d633b2c89510.png)](https://www.youtube.com/watch?v=LkFNuotJEUM)

<br>

## `Video Presentation`

> This material provides `more information` about this library and the `playground project`.

https://user-images.githubusercontent.com/51070104/203486210-db744130-4243-4ccb-87ca-17556952a276.mp4

<br />

## Why `Django Material Kit`

- Modern `Bootstrap 5` Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`
- ALL `UI KIT` pages available

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install django-theme-material-kit
// OR
$ pip install git+https://github.com/app-generator/django-theme-material-kit.git
```

<br />

> Add `theme_material_kit` application to the `INSTALLED_APPS` setting of your Django project `settings.py`:

```python
INSTALLED_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",

    'theme_material_kit',          # <-- NEW 
]
```

<br />

> Update project `settings.py` file to include (at the end of the file):

```python
LOGIN_REDIRECT_URL = '/'
EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `theme_material_kit` urls in your Django Project `urls.py` file.

```python
from django.urls import path, include              # <-- UPD with 'include' directive

urlpatterns = [
    ...
    path('', include('theme_material_kit.urls')),  #  <-- NEW
]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

<br />

## Screenshots

> [Django Theme Material Kit](https://github.com/app-generator/django-theme-material-kit) - `Cover`

![Django Theme Material Kit - Cover](https://user-images.githubusercontent.com/51070104/203402055-6c29dce8-ee03-4f43-89fb-4673e2e32b44.jpg)

<br />

> [Django Theme Material Kit](https://github.com/app-generator/django-theme-material-kit) - `Author page`

![Django Theme Material Kit - Author](https://user-images.githubusercontent.com/51070104/203402231-fc44eaa0-3a90-44b4-ad6d-34e3025ce908.jpg)

<br />

> [Django Theme Material Kit](https://github.com/app-generator/django-theme-material-kit) - Team Component

![Django Theme Material Kit - Team Component](https://user-images.githubusercontent.com/51070104/203402322-4d77ab42-6ef9-4d17-b09e-5f1b7e57e9e9.jpg)

<br />

---
**[Django Theme Material Kit](https://github.com/app-generator/django-theme-material-kit)** - Modern Theme provided by **[AppSeed](https://appseed.us/)**
