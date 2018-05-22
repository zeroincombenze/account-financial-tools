[![Build Status](https://travis-ci.org/zeroincombenze/account-financial-tools.svg?branch=9.0)](https://travis-ci.org/zeroincombenze/account-financial-tools)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/account-financial-tools/badge.svg?branch=9.0)](https://coveralls.io/github/zeroincombenze/account-financial-tools?branch=9.0)
[![codecov](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/9.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/9.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-9.svg)](https://github.com/OCA/account-financial-tools/tree/9.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-9.svg)](http://wiki.zeroincombenze.org/en/Odoo/9.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-9.svg)](http://wiki.zeroincombenze.org/en/Odoo/9.0/man/FI)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-9.svg)](http://erp9.zeroincombenze.it)


























































[![en](http://www.shs-av.com/wp-content/en_US.png)](http://wiki.zeroincombenze.org/it/Odoo/7.0/man)

Automatic creation of fiscal year sequences
===========================================

This module adds the possibility to use the %(fy)s placeholder
in sequences. %(fy)s is replaced by the fiscal year code when
using the sequence.

The first time the sequence is used for a given fiscal year,
a specific fiscal year sequence starting at 1 is created automatically.

The module also replaces %(year)s by %(fy)s in the default prefix
for new journals, assuming it is a safer default.

Caveat

/!\ If you change %(year)s to %(fy)s on a sequence that has
already been used for the current fiscal year, make sure to manually
create the fiscal year sequence for the current fiscal year and
initialize it's next number to the correct value.
For this reason, the module will forbid the user to change
a sequence from %(year)s to %(fy)s if it's next number is > 1.


Installation
------------





Configuration
-------------





Usage
-----






Known issues / Roadmap
----------------------





Bug Tracker
-----------






Bugs are tracked on `GitHub Issues <https://github.com/OCA/account-financial-tools/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed feedback
`here <https://github.com/OCA/account-financial-tools/issues/new?body=module:%20account_auto_fy_sequence%0Aversion:%208.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.


Credits
-------






Author:

* Stéphane Bidoul (ACSONE)






### Contributors






* Laetitia Gangloff (ACSONE)

[//]: # (copyright)

----

**Odoo** is a trademark of [Odoo S.A.](https://www.odoo.com/) (formerly OpenERP, formerly TinyERP)

**OCA**, or the [Odoo Community Association](http://odoo-community.org/), is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

**zeroincombenze®** is a trademark of [SHS-AV s.r.l.](http://www.shs-av.com/)
which distributes and promotes **Odoo** ready-to-use on its own cloud infrastructure.
[Zeroincombenze® distribution](http://wiki.zeroincombenze.org/en/Odoo)
is mainly designed for Italian law and markeplace.
Everytime, every Odoo DB and customized code can be deployed on local server too.

[//]: # (end copyright)

[//]: # (addons)

[//]: # (end addons)

[![chat with us](https://www.shs-av.com/wp-content/chat_with_us.gif)](https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b)
