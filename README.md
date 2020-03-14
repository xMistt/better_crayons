Better Crayons: Text UI colors for Python.
===================================

[![pypi](https://img.shields.io/pypi/v/better_crayons.svg)](https://pypi.python.org/pypi/better_crayons)
[![build](https://travis-ci.com/xMistt/better_crayons.svg?branch=master)](https://pypi.python.org/pypi/better_crayons)
[![license](https://img.shields.io/pypi/l/better_crayons.svg)](https://pypi.python.org/pypi/better_crayons)
[![wheel](https://img.shields.io/pypi/wheel/better_crayons.svg)](https://pypi.python.org/pypi/better_crayons)
[![python](https://img.shields.io/pypi/pyversions/better_crayons.svg)](https://pypi.python.org/pypi/better_crayons)

This module is really simple, it gives you colored strings for terminal
usage. Included colors are ``red``, ``green``, ``yellow``, ``blue``, ``black``, ``magenta``, ``cyan``, ``white``, and ``normal`` ( as well as ``clean`` and ``disable``).

**Better Crayons** is nice because it automatically wraps a given string in both the foreground color, as well as returning to the original state after the string is complete. Most terminal color libraries make you manage this yourself.


![example](https://i.imgur.com/eob4G6m.png)

Arguments include ``always=True`` and ``bold=True``.

Features
--------

- If you call ``disable()``, all future calls to colors will be ignored.
- If you call ``normal()``, color is reset to default foreground color
- If the current process is not in a TTY (e.g. being piped), no colors will be displayed.
- Length of ColoredStrings can be properly calculated.
- Powered by colorama.

Usage is simple
---------------

    # red is red, white is white.
    >>> print('{} white'.format(better_crayons.red('red')))
    red white

That's it!

Installation
------------

    $ pip install better_crayons
