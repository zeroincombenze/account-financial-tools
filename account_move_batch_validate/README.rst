[![Build Status](https://travis-ci.org/zeroincombenze/account-financial-tools.svg?branch=9.0)](https://travis-ci.org/zeroincombenze/account-financial-tools)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/account-financial-tools/badge.svg?branch=9.0)](https://coveralls.io/github/zeroincombenze/account-financial-tools?branch=9.0)
[![codecov](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/9.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/9.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-9.svg)](https://github.com/OCA/account-financial-tools/tree/9.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-9.svg)](http://wiki.zeroincombenze.org/en/Odoo/9.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-9.svg)](http://wiki.zeroincombenze.org/en/Odoo/9.0/man/FI)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-9.svg)](http://erp9.zeroincombenze.it)
























































[![en](http://www.shs-av.com/wp-content/en_US.png)](http://wiki.zeroincombenze.org/it/Odoo/7.0/man)

    :alt: License

Account Move Batch Validate
===========================

This module provides a wizard to post many Journal Entries in batch. it
uses the queue system introduced by the Odoo Connector to handle a
big quantity of moves in batch.

The module account_default_draft_move introduces a workflow where the
Journal Entries are always entered in Odoo in draft state, and the
posting happens later, for example at the end of the period. The core
account module provides a wizard to post all the moves in the period,
but that is problematic when there are many moves.

The posting of a move takes some time, and doing that synchronously,
in one transaction is problematic.

In this module, we leverage the power of the queue system of the
Odoo Connector, that can be very well used without other concepts
like Backends and Bindings.

This approach provides many advantages, similar to the ones we get
using that connector for e-commerce:

- Asynchronous: the operation is done in background, and users can
  continue to work.
- Dedicated workers: the queued jobs are performed by specific workers
  (processes). This is good for a long task, since the main workers are
  busy handling HTTP requests and can be killed if operations take
  too long, for example.
- Multiple transactions: this is an operation that doesn't need to be
  atomic, and if a line out of 100,000 fails, it is possible to catch
  it, see the error message, and fix the situation. Meanwhile, all
  other jobs can proceed.


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
`here <https://github.com/OCA/account-financial-tools/issues/new?body=module:%20account_move_batch_validate%0Aversion:%208.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.


Credits
-------











### Contributors






* Leonardo Pistone <leonardo.pistone@camptocamp.com>
* Nicolas Bessi <nicolas.bessi@camptocamp.com>
* Rudolf Schnapka <rs@techno-flex.de>
* Stéphane Bidoul (ACSONE) <stephane.bidoul@acsone.eu>
* Adrien Peiffer (ACSONE) <adrien.peiffer@acsone.eu>

### Funders

### Maintainer










.. image:: http://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: http://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose mission is to support the collaborative development of Odoo features and promote its widespread use.

To contribute to this module, please visit http://odoo-community.org.

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
