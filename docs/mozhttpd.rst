Serving up content to be consumed by the browser
================================================

I know, right? ANOTHER Python HTTP server? In all seriousness, we
weren't able to find anything out there that was fast enough, flexible
enough, and easy-to-use enough for our needs. So we created our own.

:mod:`mozhttpd` --- Simple webserver
------------------------------------

Mozhttpd is a simple http webserver written in python.

The server is based on python standard library modules such as 
SimpleHttpServer, urlparse, etc. The ThreadingMixIn is used to 
serve each request on a discrete thread.

While mozhttpd is often used to serve static files, dynamic handling
may be specified by a dictionary of urlhandlers.
An example of their use may be found in Eideticker.

Some existing uses of mozhttpd:

  Peptest_

  Eideticker_

  Talos_

.. _Peptest: https://github.com/mozilla/peptest/

.. _Eideticker: https://github.com/mozilla/eideticker/

.. _Talos: http://hg.mozilla.org/build/


.. automodule:: mozhttpd
   :members:

.. autoclass:: MozHttpd
   :members:
