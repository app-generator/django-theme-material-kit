# [Django Theme Material Kit](https://github.com/app-generator/django-theme-material-kit)

Modern template for **Django** coded on top of **Material Kit**, an open-source `Boostrap 5` design from `Creative-Tim`. 

<br>

**Links & Resources**

- UI Kit: [Material Design BS5](https://www.creative-tim.com/product/material-kit?AFFILIATE=128200) `v3.0.3` by Creative-Tim
- [Django Theme MKit](https://github.com/app-generator/django-theme-mkit-playground) - `playground project` 

<br />

![Material Kit - Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/167396765-c88b7a95-155f-4236-8691-7b80fa2d9cd9.png)

<br>

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

> Add `theme_material_kit` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

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

## How to use the theme

> Ordinary users set up

## Screenshots

@todo

<br />

---
**[Django Admin Material](https://github.com/app-generator/django-admin-material-dashboard)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
