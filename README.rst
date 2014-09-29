resttest
========

Testing reStructuredText support on GitHub \*.rst files

Default roles
-------------

==================================  =============  ===============  =========
         Normal text                One backslash  Two backslashes   Comment
==================================  =============  ===============  =========
:code:`code role`                   c:\temp\dir    c:\\temp\\dir
:literal:`literal`                  c:\temp\dir    c:\\temp\\dir
:emphasis:`emphasis`                c:\temp\dir    c:\\temp\\dir
:strong:`strong`                    c:\temp\dir    c:\\temp\\dir
`single backticks                   c:\temp\dir    c:\\temp\\dir    By default alias for title-reference
``literal using duoble backticks``  c:\temp\dir    c:\\temp\\dir
*emphasis using asterisks*          c:\temp\dir    c:\\temp\\dir
**strong using double asterisks**   c:\temp\dir    c:\\temp\\dir
==================================  =============  ===============  =========

Customized roles
----------------

.. default-role:: code
.. role:: custom
.. role:: inherit(emphasis)

==================================  =============  ===============  =========
         Normal text                One backslash  Two backslashes   Comment
==================================  =============  ===============  =========
:custom:`custom role`               c:\temp\dir    c:\\temp\\dir
:inherit:`inheriting role`          c:\temp\dir    c:\\temp\\dir
`single backtics`                   c:\temp\dir    c:\\temp\\dir    Default role changd to code.
==================================  =============  ===============  =========

Non-existing roles
------------------

- :nonex:`non-existing role`
