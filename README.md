# Django template for a new django CMS 4 project

A Django template for a typical django CMS installation with no 
special bells or whistles. It is supposed as a starting point 
for new projects.

If you prefer a different set of template settings, feel free to 
create your own templates by cloning this repo.

To install django CMS 4 by hand type the following commands:

1. Create virtual environment and activate it
   ```
   python3 -m venv .venv
   source .venv/bin/activate
   ```
2. Install Django, django CMS and other required packages
   ```
   pip install django-cms
   ```
3. Create project `<<project_name>>` using this template
   ```
   djangocms <<project_name>>
   cd <<project_name>>
   ```
4. Run testserver
   ```
   ./manage.py runserver
   ```
