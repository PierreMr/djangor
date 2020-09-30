# Djangor

## Django

- `https://homecreditml.herokuapp.com/`
- `django-admin startproject mysite`

## Heroku

- Create `Procfile` at the root of your repository
  - Insert `web: gunicorn myproject.wsgi`
- `pip install gunicorn`
- `pip install django-heroku`
- `settings.py`
  - At the top `import django_heroku`
  - At the bottom `django_heroku.settings(locals())`
- `pip freeze > requirements.txt`
- `heroku git:clone -a mysite`
- `git push heroku master`