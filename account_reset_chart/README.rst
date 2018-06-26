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

Account chart reset
===================

Adds a method to the company to remove its chart of accounts, including all
related transactions, journals etc. By necessity, this process also removes
the company's bank accounts as they are linked to the company's journals and
the company's payment orders and payment modes if the payment module is
installed.

As a result, you can then reconfigure the company chart of account with the
same or a different chart template.

Installation
------------





Configuration
-------------





Usage
-----






=====

To prevent major disasters when this module is installed, no interface is
provided. Please run through xmlrpc, for instance using erppeek: ::

    import erppeek
    
    host = 'localhost'
    port = '8069'
    admin_pw = 'admin'
    dbname = 'openerp'
    
    client = erppeek.Client('http://%s:%s' % (host, port))
    client.login('admin', admin_pw, dbname)
    client.execute('res.company', 'reset_chart', 1)

Known issues / Roadmap
----------------------






This should work with the standard accounting modules installed. All sorts of
combinations with third party modules are imaginable that would require
modifications or extensions of the current implementation.

Sequences are not reset during the process.


Bug Tracker
-----------






Bugs are tracked on `GitHub Issues <https://github.com/OCA/account-financial-tools/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed feedback
`here <https://github.com/OCA/account-financial-tools/issues/new?body=module:%20account_reset_chart%0Aversion:%208.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.


Credits
-------











### Contributors






* Stefan Rijnhart <stefan@therp.nl>

Icon courtesy of Alan Klim (CC-BY-20) -
https://www.flickr.com/photos/igraph/6469812927/

### Funders

### Maintainer










.. image:: http://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: http://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

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
