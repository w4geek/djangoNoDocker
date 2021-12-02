# djangoNoDocker
Django NoDocker

Inicialización del proyecto:

1. Instalar Python 3+

2. Instalar paquetes en "requirements.txt"

pip install -r requirements.txt

3. Instalar MySql e iniciar servicio.

4. Ejecutao el initial.sql para crear esquema de django

## Creamos nuestro proyecto de django

django-admin startproject {NOMBRE PROYECTO} (nombre espacio punto)

## Modificamos Settings.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'django',
        'USER': 'userdjango',
        'PASSWORD': 'passworddjango',
        'HOST': 'localhost',
        'PORT': 3306,
    }

## Ahora ya podemos crear la app con el comando:

python manage.py startapp {REEMPLAZAR POR NOMBRE DE APP}

## Recordar correr comando

python manage.py migrate

## Ejecutar la app de django con el comando:

python manage.py runserver 0.0.0.0:8000
