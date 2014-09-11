resttest
========

Testing reStructuredText support on GitHub \*.rst files

Roles
-----

Default roles:

- :code:`code role`
- :literal:`literal`
- :emphasis:`emphasis`
- :strong:`strong`
- `single backticks (by default alias for title-reference)`
- ``literal using duoble backticks``
- *emphasis using asterisks*
- **strong using double asterisks**

Customization:

.. default-role:: code
.. role:: custom
.. role:: inherit(emphasis)

- :custom:`custom role`
- :inherit:`inheriting role`
- `single backtics (after changing default role to code)`

Errors:

- :nonex:`non-existing role`
