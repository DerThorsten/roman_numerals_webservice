=====
Usage
=====

After installing the python package :code:`roman_numerals_webservice`
the webserver can be started with the following command

.. code-block:: shell

    roman_numerals_webservice

When the server is running requests can be send to the webservice.
On a Unix system this can be done with :code:`curl`

.. code-block:: shell

    $ curl -d '{"roman" : "XL"}' -H "Content-Type: application/json" -X POST http://localhost:8080/roman_to_arabic
    {\"arabic\": 40}"

.. code-block:: shell

    $ curl -d '{"arabic" : 1987}' -H "Content-Type: application/json" -X POST http://localhost:8080/arabic_to_roman
    "{\"roman\": \"MCMLXXXVII\"}"


To use roman_numerals_webservice in a project::

    import roman_numerals_webservice
