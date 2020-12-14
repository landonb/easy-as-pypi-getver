############
Installation
############

.. |virtualenv| replace:: ``virtualenv``
.. _virtualenv: https://virtualenv.pypa.io/en/latest/

.. |workon| replace:: ``workon``
.. _workon: https://virtualenvwrapper.readthedocs.io/en/latest/command_ref.html?highlight=workon#workon

To install system-wide, run as superuser::

    $ pip3 install easy-as-pypi-getver

To install user-local, simply run::

    $ pip3 install -U easy-as-pypi-getver

To install within a |virtualenv|_, try::

    $ mkvirtualenv easy-as-pypi-getver
    (easy-as-pypi-getver) $ pip install release-ghub-pypi

To develop on the project, link to the source files instead::

    (easy-as-pypi-getver) $ deactivate
    $ rmvirtualenv easy-as-pypi-getver
    $ git clone git@github.com:tallybark/easy-as-pypi-getver.git
    $ cd easy-as-pypi-getver
    $ mkvirtualenv -a $(pwd) --python=/usr/bin/python3.8 easy-as-pypi-getver
    (easy-as-pypi-getver) $ make develop

After creating the virtual environment,
to start developing from a fresh terminal, run |workon|_::

    $ workon easy-as-pypi-getver
    (easy-as-pypi-getver) $ ...

