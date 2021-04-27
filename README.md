# Django + DjangoRESTFramework + Vue Application

## Installation

`pip install django djangorestframework django-cors-headers djoser pillow stripe`

On `settings.py` file:

1. Put `rest_framework`, `rest_framework.authtoken`, `corsheaders` and `djoser` in `INSTALLED_APPS`.

2. Put `corsheaders.middleware.CorsMiddleware` in `MIDDLEWARE`.

3. Put `127.0.0.1` or `localhost` in `ALLOWED_HOST` list.

4. Create new variable `CORS_ALLOWED_ORIGINS` with `http://localhost:8080` value in list type.

5. Add `path('api/v1/', include('djoser.urls'))` and `path('api/v1/', include('djoser.urls.authtoken'))` in `urls.py`.

6. Run `python manage.py makemigrations`.

7. Run `python manage.py migrate`.

8. Create superuser by running `python manage.py createsuperuser`.

9. To run the server, run `python manage.py runserver` command.
