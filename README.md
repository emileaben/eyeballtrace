# eyeballtrace
This is a proof of concept for doing traceroutes from networks with significant user populations in a country.
THIS TOOL IS A PROTOTYPE, YOUR MILEAGE MAY VARY.


Usage:

    eyeballtrace -c <country>  <target>

<country> is an ISO 2 letter country code.
<target> can be a hostname or IPv4 address.
 

Installation:

This tools depends on a couple of python modules that can be installed with pip like this:

    pip install -r requirements.txt

If you don't have pip, instructions are available at: https://pip.pypa.io/en/latest/installing.html

For creating measurements with RIPE Atlas this tool needs an atlas api key in ~/.atlas/auth . Instructions on how to create such key are available at: XXX , if you have the key:

    mkdir -p ~/.atlas/
    echo "<YOUR_KEY_HERE>" > ~/.atlas/auth
    chmod 700 ~/.atlas/
    chmod 600 ~/.atlas/auth

Of course you'll need RIPE Atlas credits to run this. Per ASN up to 3 probes are selected that do a one-off traceroute, so for a country with 10 eyeball ASNs with probes that would be a maximum of 10x3x60 = 1800 credits for a single run of this tool.

THIS TOOL IS A PROTOTYPE, YOUR MILEAGE MAY VARY

Note: This has been tested on OSX 10.9.5 with Python 2.7.9
