# Django template for a new django CMS project

A Django template for a typical django CMS installation. It is intended as a
starting point for new projects created with the `djangocms` command.

If you prefer a different set of template settings, feel free to
create your own templates by cloning this repo.

## Usage

To install django CMS type the following commands:

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

Note: If you run into a problem of missing dependencies, please
update `pip` using `pip install -U pip` before running the
`djangocms` command.

## Template options

The `djangocms` command reads the supported template options from
`djangocms_install_rules.json`. Current options include:

- `--mode traditional|headless|hybrid`
- `--versioning` / `--no-versioning`
- `--moderation` / `--no-moderation`
- `--alias` / `--no-alias`
- `--stories` / `--no-stories`
- `--history` / `--no-history`

Example:

```
djangocms <<project_name>> --mode hybrid --history
```

## Installation rules

`djangocms_install_rules.json` is also used when adding django CMS to an
existing Django project:

```
djangocms . --mode hybrid --history
```

The file describes command option metadata, apps, middleware, settings, URL
patterns, package requirements, and the conditions under which they apply.
`djangocms_install_rules.schema.v1.json` defines the JSON schema for that file.
