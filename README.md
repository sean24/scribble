# scribble

## Front-end

MVC framework: angular from Google, react from Facebook, ember, etc. Include from CDNs.

    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js"></script>

jquery: DOM manipulation, AJAX, etc. Include from one of the CDN

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
    <script src="https://ajax.aspnetcdn.com/ajax/jQuery/jquery-3.2.1.min.js"></script>
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>

bootstrap: include from the CDN

    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta/js/bootstrap.min.js"></script>

Code editor: sublime, bracket

JS runtime: node.js from Chrome

JS packaging: npm

## Back-end

Frameworks: ruby on rails, Django (python), etc.

## Django

Python 3 and pip should already been installed.

    python3 --version
    python3 -m pip --version

Install django

    pip3 install django
    python3 -m django --version

Create a project `olympus`

    django-admin startproject olympus

Create an app `polls` as per https://docs.djangoproject.com/en/1.11/intro/tutorial01/[tutorial]

    cd olympus
    python3 manage.py startapp polls
    # edit files

Change to the directory that contains `manage.py`, start the server then in
browser go to `https://127.0.0.1:8000/polls`.

    cd olympus
    python3 manage.py runserver

Change timezone to `America/Toronto` in `olympus/settings.py`.

Create tables used by installed apps.

    python3 manage.py migrate

Check the tables

    sqlite3 db.sqlite3
    sqlite> .tables
    sqlite> .exit

