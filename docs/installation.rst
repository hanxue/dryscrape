.. highlight:: none

Installation
============

Prequirements
-------------

Before installing dryscrape_, you need to install some software it depends on:

* Qt4_, QtWebKit_
* lxml_
* pip_

On Ubuntu you can do that with one command (the ``#`` indicates that you need root privileges for
this):

::

  # apt-get install libqt4-dev libqtwebkit-dev qt4-qmake build-essential \
                    python-lxml python-pip

On other operating systems, you can use pip_ to install lxml (though you might
have to install libxml and the Python headers first).

pip
---
If you already have python pip available on your system

::
  
  $ pip install dryscrape
  

Build from source
---------

First, get a copy of dryscrape_ using Git:

::

  $ git clone https://github.com/niklasb/dryscrape.git dryscrape
  $ cd dryscrape

To install dryscrape, you first need to install webkit-server_. You can use
pip_ to do this for you (while still in the dryscrape directory).

::

  # pip install -r requirements.txt

If you want, you can of course also install the dependencies manually.

Afterwards, you can use the ``setup.py`` script included to install dryscrape:

::

  # python setup.py install

Note that dryscrape is written for Python 2.7+, so make sure that you use both the
``python`` and ``pip`` commands in the right version.

.. _QT4: http://qt.nokia.com/
.. _QtWebKit: http://developer.qt.nokia.com/doc/qt-4.8/qtwebkit.html
.. _lxml: http://lxml.de/
.. _webkit-server: https://github.com/niklasb/webkit-server/
.. _pip: http://pypi.python.org/pypi/pip
.. _dryscrape: https://github.com/niklasb/dryscrape/
