Installation
==============================================================================

It is recommended to work out of a
[VirtualENV](http://pypi.python.org/pypi/virtualenv) during development of
your application, which is reference throughout this documentation. VirtualENV
is easily installed on most platforms either via PIP or by your OS
distributions packaging system (Yum, Apt, Brew, etc).

Installation
------------------------------------------------------------------------------

*Installing Stable Versions from PyPI:*

```bash
$ pip install cement
```

*Installing Development Versions from Git:*

```bash
$ pip install -e git+git://github.com/datafolklabs/cement.git#egg=cement
```


Running Tests
------------------------------------------------------------------------------

To run tests, you will need to ensure any dependent services are running (for
example Memcached), and then do the following from the root of the source:

```bash
# Start services
$ memcached &

# Python 2.x
$ pip install -r requirements-dev.txt

# Python 3.x
$ pip install -r requirements-dev-py3.txt

$ python setup.py nosetests
```


Building Documentation
------------------------------------------------------------------------------

To build this documentation, do the following from the root of the source:

```bash
$ python setup.py build_sphinx
```
