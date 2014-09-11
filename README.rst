resttest
========

Testing reStructuredText support on GitHub \*.rst files

Roles
-----

Default roles:

- :code:`code role`
- :literal:`literal role`
- `single backticks (by default alias for title-reference role)`
- ``double backticks (alias for literal role)``

Customization:

.. default-role:: code
.. role:: custom
.. role:: inherit(emphasis)

- `single backtics (after changing default role to code)`
- :custom:`custom role`
- :inherit:`inheriting role`

Errors:

- :nonex:`non-existing role`
