# first-django
Basic API using DJango REST with some CRUD

# Commands and steps
- django-admin startproject firstproject
- python manage.py startapp api (in firstproject folder)
- In firstproject/settings.py, in INSTALLED_APPS, add:
  - 'rest_framework'
  - 'api'
- Define tables in api/models.py
- Execute manager.py with parameter 'makemigrations' to create migration script and so execute with 'migrate' 
to really migrate
- Define how to transform models in JSON for REST API in api/serializer
- Define endpoint functions in api/views.py
- Define the endpoint paths to make API request in api/urls.py, in urlpatterns.
- Include the defined endpoints in firstproject/urls, in urlpatterns.
- To start server, execute manager.py with parameter 'runserver'