Dirbpy
--------

.. image:: https://img.shields.io/pypi/v/dirbpy.svg
    :target: https://pypi.org/project/dirbpy/
.. image:: https://img.shields.io/pypi/pyversions/dirbpy.svg
    :target: https://pypi.org/project/dirbpy/
.. image:: https://travis-ci.org/marcolivierbouch/dirbpy.svg?branch=master
    :target: https://travis-ci.org/marcolivierbouch/dirbpy

Description
-----------
Dirbpy - URL Bruteforcer

This is a new version of dirb but in python. This version is faster than the normal version in C because it uses thread. Dirbpy is a Web Content Scanner. It looks for hidden Web Objects. It basically works by launching an attack based on a dictionary against a web server and analyzing the response.

Link to the original dirb: https://github.com/v0re/dirb

Install with pip
----------------
``pip install dirbpy``

Fish completions
----------------
``git clone https://github.com/marcolivierbouch/dirbpy.git``

``cd dirbpy``

``sudo cp dirbpy.fish /usr/share/fish/completions``

Dirbpy with Docker
------------------
Build the Docker image

``docker build . -t <name-image>``

Build Example

``docker build . -t myusername/dirbpy``

Run the container as if you were running the normal dirb command using the docker run option "--rm" (container will be automatically removed after the command has completed its execution)

``docker run --rm myusername/dirbpy [OPTIONS]``

Command Example

``docker run --rm myusername/dirbpy -o https://raw.githubusercontent.com/danielmiessler/SecLists/master/Discovery/Web-Content/common.txt -u https://[....].com"



Recommendations
---------------
I recommend using the SecLists: https://github.com/danielmiessler/SecLists
