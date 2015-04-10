# django-gae-backend
Porting Google App Engine rdbms backend to newly Django (>= 1.6)

The rdbms backend on App Engine SDK is not working on newly Django (>= 1.6). <br>
This package porting the backend to newly Django and has been tested on Django 1.8.

How to use:
* Put django_gae_backend under your project folder
* Add django_gae_backend to google's namespace
```
import os
from google.storage.speckle.python.django import backend
backend.__path__.insert(0, os.path.join(os.path.dirname(__file__), os.pardir, 'django_gae_backend'))
```
