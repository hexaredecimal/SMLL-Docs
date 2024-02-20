Usage
=====

.. _installation:

Installation
------------
To use *SMLL* you must compile it first. Use the following commands to install
.. note::
   I assume that you have already cloned the git repo, if not do so by cloning this link. 
   https://github.com/hexaredecimal/ML.git

.. code-block:: console
   cd ML
   cargo build
   ./target/debug/smll --help

After this you should have a working compiler front-end, now the problem is wheather you have a supported JAVA compiler for
compiling the output java files. Execute the following code to verify your java compiler. 

.. code-block:: console
  java --version

.. note::
  On my machine this is the output:
  java 21.0.1 2023-10-17 LTS
  Java(TM) SE Runtime Environment (build 21.0.1+12-LTS-29)
  Java HotSpot(TM) 64-Bit Server VM (build 21.0.1+12-LTS-29, mixed mode, sharing)

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

