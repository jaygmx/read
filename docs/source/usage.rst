Usage
=====

.. _installation:

Installation
------------

To use Jay, first install it using pip:

.. code-block:: console

   (.venv) $ pip install jay

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``jay.get_random_ingredients()`` function:

.. autofunction:: jay.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`jay.get_random_ingredients`
will raise an exception.

.. autoexception:: jay.InvalidKindError

For example:

>>> import jay
>>> jay.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

