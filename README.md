# django-test
Test django framework


# Creation du projet
django-admin startproject project_name

## Configuration Vhost Apache2

<code>
$ apt-get install libapache2-mod-wsgi
</code>

Créer un vhost avec les infos suivantes:
<code>

WSGIDaemonProcess djangotest python-path=/var/www/django_test/
WSGIProcessGroup djangotest
WSGIScriptAlias / /var/www/django_test/wsgi.py
</code>

Configurer ensuite les hôtes depuis settings.py

## Créer une app

<code>
python manage.py startapp testapp
</code>
