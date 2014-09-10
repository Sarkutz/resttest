resttest
========

Testing reStructuredText support on GitHub *.rst files

Roles
-----

Default roles:

- `single backticks (default role)`
- ``double backticks (alias for literal role)`
- :code:`code role`

Customization:

.. default-role:: code
.. role:: custom

- `single backtics (after changeing default role to code)`
- :custom:`custom role`

Errors:

- :nonex:`non-existing role`
