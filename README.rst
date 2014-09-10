resttest
========

Testing reStructuredText support on GitHub ``*.rst`` files

Roles
-----

Default roles:

- `single backticks (default role)`
- ``double backticks (alias for literal role)``
- :code:`code role`
- :literal:`literal role`

Customization:

.. default-role:: code
.. role:: custom

- `single backtics (after changing default role to code)`
- :custom:`custom role`

Errors:

- :nonex:`non-existing role`
