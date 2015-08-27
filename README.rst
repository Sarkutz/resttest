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

Tables
------

List-table
~~~~~~~~~~

.. list-table:: A title
    :widths: 1, 2, 2, 5 
    :header-rows: 1

    * - ID
      - Type
      - Priority
      - Summary
    * - #42
      - Bug
      - Critical
      - Just testing here, nothing more
    * - #1
      - Enhancement
      - Low
      - Testing, testing, 1 2 3
