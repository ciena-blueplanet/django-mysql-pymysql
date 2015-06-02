django-mysql-pymysql
====================

This is a Django database backend for MySQL, using the PyMySQL database adapter. It is intended to be a drop-in replacement for the built-in MySQLdb backend, and leverages quite a bit of its code.

It is currently experimental, and has been tested with Django 1.8.


Requirements
------------

* Django trunk or Py3k Branch
* PyMySQL (patches here: https://github.com/clelland/PyMySQL)

Installation
------------

1. Clone and install into your site-packages directory:

        $ git clone https://github.com/clelland/django-mysql-pymysql
        $ cd django-mysql-pymysql
        $ python setup.py install

2. Edit your settings file:

        DATABASES = {
            'default': {
                'ENGINE': 'mysql_pymysql',
                'HOST': ...,
                'USER': ...,
                'PASSWORD': ...,
            }
        }


3. You're done.
