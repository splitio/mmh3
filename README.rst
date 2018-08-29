murmurhash3
===========

:Version: 1.0.3
:Download: http://pypi.python.org/pypi/splitmmh3/
:Source: http://github.com/splitio/mmh3
:Keywords: hash, MurmurHash

murmurhash3 is a Python library for MurmurHash (MurmurHash3), a set of fast and
robust hash functions. This library is a Python extension module written in C.

Supports Python >= 2.7


Usage
=====

Install::

    pip install splitmmh3

Usage::

    pip install splitmmh3

    >>> import splitmmh3 as mmh3
    >>> mmh3.hash('foo')  # 32-bit signed int
    -156908512
    >>> mmh3.hash64('foo')  # two 64-bit signed ints (the 128-bit hash sliced in half)
    (-2129773440516405919, 9128664383759220103)
    >>> mmh3.hash128('foo')  # 128-bit signed int
    168394135621993849475852668931176482145
    >>> mmh3.hash_bytes('foo')  # 128-bit value as bytes
    'aE\xf5\x01W\x86q\xe2\x87}\xba+\xe4\x87\xaf~'
    >>> mmh3.hash('foo', 42)  # uses 42 for its seed
    -1322301282


License
=======

Public Domain


Authors
=======

MurmurHash3 was created by Austin Appleby

- http://code.google.com/p/smhasher/
