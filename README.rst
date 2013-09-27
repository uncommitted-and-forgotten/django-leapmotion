Django Leap Motion
==================

Controll a django app with gestures using the Leap Motion device. 

For more information about the controller, please visit [https://www.leapmotion.com/](https://www.leapmotion.com/) and for more development ressources, protocoll info, etc. visit [http://js.leapmotion.com/](http://js.leapmotion.com/).



Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    $ pip install django-leapmotion

To get the latest commit from GitHub

.. code-block:: bash

    $ pip install -e git+git://github.com/philippeowagner/django-leapmotion.git#egg=leapmotion

TODO: Describe further installation steps (edit / remove the examples below):

Add ``leapmotion`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'leapmotion',
    )

Add the ``leapmotion`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^leapmotion/', include('leapmotion.urls')),
    )

Don't forget to collect the static media.

.. code-block:: bash

    ./manage.py collectstatic 


Usage
-----

You need to have the LEAP SDK / WebSocket server installed (SDK version 0.7.1+). 
You also need a modern browser. 


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    $ mkvirtualenv -p python2.7 django-leapmotion
    $ python setup.py install
    $ pip install -r dev_requirements.txt

    $ git co -b feature_branch master
    # Implement your feature and tests
    $ git add . && git commit
    $ git push -u origin feature_branch
    # Send us a pull request for your feature branch
