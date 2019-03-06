# Overview

A tiny python (non reactive) charm that demonstrates the "hook" concept for Juju.

This charm runs only on:
 * Ubuntu series with python3 (bionic, disco, etc.)
 * Systems with ability to do 'pip install' from network

## What it does
This charm starts with :
 * installing "python3-pip" in [hooks/setup.py] and 'charmhelpers'

 * Then goes ahead and acts on the hooks in the hooks directory as part of the juju event cycle.

This charm is for practice and study only. Its really not very useful for other that this.

# Usage

```
charm pull https://jujucharms.com/new/u/erik-lonroth/tiny-python && juju deploy ./tiny-python
```

# Configuration

None


# Contact Information

Erik Lönroth <erik.lonroth@gmail.com>
