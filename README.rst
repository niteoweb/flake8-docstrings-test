Prepare
=======

.. code-block:: bash

	$ git clone git@github.com:niteoweb/flake8-docstrings-test.git
	$ cd flake8-docstrings-test
	$ virtualenv .
	$ pip install flake8-docstrings pydocstyle

Test
====

.. code-block:: bash

	$ bin/pydocstyle foo.py 
	# OK: no output, because errors are ignored in .pydocstyle

	$ bin/flake8 foo.py
	foo.py:1:1: D100 Missing docstring in public module
	foo.py:1:1: D103 Missing docstring in public function
	# BUG: configuration in .pydocstyle is ignored
