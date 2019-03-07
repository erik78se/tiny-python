# Overview

A tiny (non reactive) charm that intends to teach about the "hook" concept for Juju.

See: https://docs.jujucharms.com/2.5/en/reference-charm-hooks

## What it does
This charm starts with :
 * Installs "python3-pip" in [hooks/setup.py] and 'charmhelpers'

 * Acts on the hooks in the hooks directory as part of the juju event cycle.

This charm is for educational purposes. You can learn about Juju hooks with this.

Check out the 'hooks' directory to learn.

# Usage

```
charm pull cs:~erik-lonroth/tiny-python  && juju deploy ./tiny-python
```

# Configuration

None

# Known limitations

Because its a python charm, this charm depends on python3 which limit to:.

 * Ubuntu series bionic, disco where python3 is default.
 * Systems with ability to do 'pip install' from network

# Contact Information

Erik Lönroth <erik.lonroth@gmail.com>
