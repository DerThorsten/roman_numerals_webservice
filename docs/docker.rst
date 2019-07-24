Docker
============

Assuming you are in the root dir of the repository,
the following will build the docker container

.. code:block:: shell

    sudo docker build -t roman_numeras_webservice .

To start the server use the following:

.. code:block:: shell

    docker run -p 8080:8080 roman_numeras_webservice


Alternatively one can use the prebuild docker image hosted at dockerhub:


.. code:block:: shell

    docker pull derthorsten/roman_numeras_webservice:latest
