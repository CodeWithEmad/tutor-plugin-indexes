Tutor Plugin Indexes
####################

This is the repository for the Tutor plugin indexes maintained by me.
A Tutor plugin index is similar to the Python Package index (PyPi) or an apt repository:
it is a reference to many plugins that can then be easily installed and enabled by Tutor.

For more information about Tutor indexes, see the `official Tutor Documentation`_.

Available Plugins
*****************

- `wordpress <https://github.com/CodeWithEmad/tutor-contrib-wordpress>`__: Integrates WordPress with Open edX
- `phpmyadmin <https://github.com/CodeWithEmad/tutor-contrib-phpmyadmin>`__: Adds phpMyAdmin database management interface

Usage
*****

Add the index with:

.. code-block:: bash

  tutor plugins index add https://raw.githubusercontent.com/CodeWithEmad/tutor-plugin-indexes/main/

Install the the following plugins from the main index:

.. code-block:: bash

    tutor plugins install wordpress
    tutor plugins install phpmyadmin

If you need to update the cache, that means, fetching the latest changes in the index, use the command ``tutor plugins update``.

You can remove the index with:

.. code-block:: bash

  tutor plugins index remove https://raw.githubusercontent.com/CodeWithEmad/tutor-plugin-indexes/main/

Contributions
*************

All contributions are welcome. feel free to open a PR or an issue.


License
*******

This software is licensed under the terms of the AGPLv3. See the `LICENSE`_ file for details.

.. _LICENSE: https://raw.githubusercontent.com/CodeWithEmad/tutor-plugin-indexes/main/LICENSE
.. _official Tutor Documentation: https://docs.tutor.edly.io/reference/indexes.html