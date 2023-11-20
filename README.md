# Django template for a new django CMS project

A Django template for a typical django CMS installation.

To install django CMS 4 by hand type the following commands:

1. Create virtual environment and activate it
   ```
   python3 -m venv .venv
   . .venv/bin/activate
   ```
2. Install Django, django CMS and other required packages
   ```
   pip install djangocms-frontend\[cms4] djangocms-versioning djangocms-alias
   ```
3. Create project `<<project_name>>` using this template
   ```
   django-admin startproject --template https://github.com/django-cms/cms-template/archive/main.zip <<project_name>>
   cd <<project_name>>
   ```
4. Create database and run checks
   ```
   ./manage.py migrate
   ./manage.py cms check
   ```
5. Create superuser
   ```
   ./manage.py createsuperuser
   ```
6. Run testserver
   ```
   ./manage.py runserver
   ```

