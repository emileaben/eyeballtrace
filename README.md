# eyeballtrace
This is a proof of concept for doing traceroutes from networks with significant user populations in a country

Usage:

    eyeballtrace -c <country>  <target>
 

Installation:

This tools depends on a couple of python modules that can be installed with pip like this:

    pip install -r requirements.txt

If you don't have pip, instructions are available at: https://pip.pypa.io/en/latest/installing.html

For creating measurements with RIPE Atlas this tool needs an atlas api key in ~/.atlas/auth . Instructions on how to create such key are available at: XXX , if you have the key:

    mkdir -p ~/.atlas/
    echo "<YOUR_KEY_HERE>" > ~/.atlas/auth
    chmod 700 ~/.atlas/
    chmod 600 ~/.atlas/auth


Note: This has been tested on OSX 10.9.5 with Python 2.7.9
