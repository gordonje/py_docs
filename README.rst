py_docs
=======

A walk-through of Python documentation tools, including:

1. Docutils and `reStructuredText <http://docutils.sourceforge.net/docs/user/rst/quickref.html>`_
2. `Sphinx <http://www.sphinx-doc.org/en/stable/>`_
3. `ReadTheDocs <https://readthedocs.org/>`_

This is a pretty good ``video tutorial <https://www.youtube.com/watch?v=oJsUvBQyHBs>``_.

Setting up
----------

Install the requirements:

.. code-block:: bash

    $ pip install -r requirements.txt


Then set up the sphinx project:

.. code-block:: bash

    $ sphinx-quickstart


This will step you through several options. You can mostly keep the defaults.


"live" html
-----------

Paste this into ``docs/Makefile``:

.. code-block:: bash
    livehtml:
        sphinx-autobuild -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
