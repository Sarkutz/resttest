================================
  GitHub reStructuredText Test
================================

This document tests various `reStructeredText <http://docutils.sourceforge.net/rst.html>`__
features when rendered on GitHub. The motivation is to test what kind of styles GitHub uses
and how different features actually work here. 

.. contents::
   :depth: 2
   :local:

Roles
=====

Testing reStructuredText support on GitHub \*.rst files

Default roles
-------------

==================================  =======================  =========================  ===========
            Normal text                  One backslash             Two backslashes        Comment
==================================  =======================  =========================  ===========
:code:`code role`                   :code:`c:\temp\dir`      :code:`c:\\temp\\dir`
:literal:`literal`                  :literal:`c:\temp\dir`   :literal:`c:\\temp\\dir`
:emphasis:`emphasis`                :emphasis:`c:\temp\dir`  :emphasis:`c:\\temp\\dir`
:strong:`strong`                    :strong:`c:\temp\dir`    :strong:`c:\\temp\\dir`
`single backticks`                  `c:\temp\dir`            `c:\\temp\\dir`            By default alias for title-reference
``literal using duoble backticks``  ``c:\temp\dir``          ``c:\\temp\\dir``          Standard alias.
*emphasis using asterisks*          *c:\temp\dir*            *c:\\temp\\dir*            Standard alias.
**strong using double asterisks**   **c:\temp\dir**          **c:\\temp\\dir**          Standard alias.
==================================  =======================  =========================  ===========

Customized roles
----------------

.. default-role:: code
.. role:: custom
.. role:: inherit(emphasis)

==========================  ======================  ========================  ===========
        Normal text              One backslash           Two backslashes        Comment
==========================  ======================  ========================  ===========
:custom:`custom role`       :custom:`c:\temp\dir`   :custom:`c:\\temp\\dir`
:inherit:`inheriting role`  :inherit:`c:\temp\dir`  :inherit:`c:\\temp\\dir`
`single backtics`           `c:\temp\dir`           `c:\\temp\\dir`           Default role changed to code.
==========================  ======================  ========================  ===========

Non-existing roles
------------------

- :nonex:`non-existing role`

Lists
=====

Unordered without indentation:

- First item
- Second
- Third

Unordered wit indentation:

  - First item
  - Second
  - Third


Ordered without indentation:

1. First item
2. Second
3. Third

Ordered wit indentation:

  1. First item
  2. Second
  3. Third

Links
=====


- Explicit target_
- `Target with spaces`_
- Links_ is implicit target
- Anonymous__ link
- `Embedded URI <http://example.com>`__
- `Embedded alias <target_>`__

.. _target: http://example.com
.. _target with spaces: http://example.com
__ http://example.com

Escaping
========

- \http://example.com
- `\http://example.com`
