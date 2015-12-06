skele-cli
=========

*A skeleton command line program in Python.*


Purpose
-------

This is a skeleton application which demonstrates how to properly structure a
Python CLI application.

I've done my best to structure this in a way that makes sense for *most* users,
but if you have any feedback, please open a Github issue and I'll take a look.

The idea with this project is that you should be able to use this as a template
for building new CLI apps.

You can fork this project and customize it to your liking, or just use it as a
reference.


Usage
-----

If you've cloned this project, and want to install the library (*and all
development dependencies*), the command you'll want to run is::

    $ pip install -e .[test]

If you'd like to run all tests for this project (*assuming you've written
some*), you would run the following command::

    $ python setup.py test

This will trigger `py.test <http://pytest.org/latest/>`_, along with its popular
`coverage <https://pypi.python.org/pypi/pytest-cov>`_ plugin.

Lastly, if you'd like to cut a new release of this CLI tool, and publish it to
the Python Package Index (`PyPI <https://pypi.python.org/pypi>`_), you can do so
by running::

    $ python setup.py sdist bdist_wheel
    $ twine upload dist/*

This will build both a source tarball of your CLI tool, as well as a newer wheel
build (*and this will, by default, run on all platforms*).

The ``twine upload`` command (which requires you to install the `twine
<https://pypi.python.org/pypi/twine>`_ tool) will then securely upload your
new package to PyPI so everyone in the world can use it!
