# Django template for a new django CMS 3.11 project

A Django template for a typical django CMS installation with no 
special bells or whistles. It is supposed as a starting point 
for new projects.

If you prefer a different set of template settings, feel free to 
create your own templates by cloning this repo.

To install django CMS 3.11 by hand type the following commands:

1. Create virtual environment and activate it
   ```
   python3 -m venv .venv
   . .venv/bin/activate
   ```
2. Install Django, django CMS and other required packages
   ```
   pip install djangocms-frontend\[cms-3]
   ```
3. Create project `<<project_name>>` using this template
   ```
   django-admin startproject --template https://github.com/django-cms/cms-template/archive/3.11.zip <<project_name>>
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

