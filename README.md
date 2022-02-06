# Overview

The tiny-python charm that use "hooks only" to deploy. Since its super small and only uses hooks, it deploys very fast.

It depends on the "charmhelpers" library which is helpful when writing charms with python.


## What it does
This charm starts with :
 * Installs "python3-pip" in [hooks/setup.py] and 'charmhelpers'

 * Acts on the hooks in the hooks directory as part of the juju event cycle.

Check out the 'hooks' directory to learn.

## Deploy from charmhub

    juju deploy tiny-python

## Deploy from  development host

Hook-only charms doesn't need to be built, so you can deploy straight from the directory:

    git clone git@github.com:erik78se/tiny-python.git
    juju deploy ./tiny-python

## Build the charm

You can build the charm if you like with charmcraft:

    git clone git@github.com:erik78se/tiny-python.git
        charmcraft build
    juju deploy ./tiny-python.charm


## Known limitations

Because its a python charm, this charm depends on python3 which limit to:

 * Ubuntu series bionic, disco where python3 is default.
 * Systems with ability to do 'pip install' from network

# Contact Information

Erik Lönroth <erik.lonroth@gmail.com>
