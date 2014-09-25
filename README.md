#Online Petition

[![Build Status](https://travis-ci.org/norrs/onlinepetition.svg?branch=master)](https://travis-ci.org/norrs/onlinepetition)
[![Coverage Status](https://coveralls.io/repos/norrs/onlinepetition/badge.png?branch=master)](https://coveralls.io/r/norrs/onlinepetition?branch=master)

Simple system for registering and validating people signing an online petition.

# Install

* Install virtualenv (on debian/ubuntu: apt-get install python-virtualenv ) 
* virtualenv --no-site-packages /path/to/store/your/virtualenv/onlinepetition
* source /path/to/virtualenv/onlinepetition/bin/activate
* pip install Django
* pip install South
* pip install ipython

## Initialize database first time

* python manage.py syncdb
* python manage.py createsuperuser (if syncdb didn't prompt you to create one)
* python manage.py migrate

## Update translation strings:
* Add or change translatable strings in template or python code
* python manage.py makemessage -l nb_NO to generate keys in norwegian language file
* Edit locale/nb_NO/LC_MESSAGES/django.po and add your translations
* python manage.py compilemessages

Your new translations are now ready to use :)

You should now be done :-)

# Note

System currently under heavy dev, please consider current code rather unstable ;-)

