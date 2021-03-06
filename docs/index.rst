.. wr documentation master file, created by
   sphinx-quickstart on Thu Apr 12 17:15:43 2012.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


wr (Weighted Random)
====================

*wr is a weighted random implementation in Python.*

``wr.choice`` can be fed with a mapping (such as dictionaries) containing a returnable (what to return) and a integer representing their respective weight.  
The key can be anything hashable but the weight must be a integer.

Optionally you may feed ``wr.choice`` with a sequence of pairs.

Functions
----------

.. automodule:: wr  
    :members:

Example
-------
::

    >>> import wr
    
    >>> data = {'cat': 60, 'dog': 30, 'bird': 10}
    >>> animal = wr.choice(data)
    >>> print animal
    cat # well, the cat had a good 60% shot at it.

Structures
----------
::

    {something_to_return: weight, something_else_to_return: weight}
    # Or as a sequence:
    [(something_to_return, weight), (something_else_to_return, weight)]

Installation
------------

Install wr with ``pip install wr`` or just `download wr.py <http://pypi.python.org/pypi/wr>`_ and place it in your project directory.

License
-------
`BSD <http://www.linfo.org/bsdlicense.html>`_

