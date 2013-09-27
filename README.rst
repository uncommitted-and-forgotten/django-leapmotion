Django Leap Motion
============

Control your app using Leap Motion

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

Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate leapmotion


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


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
