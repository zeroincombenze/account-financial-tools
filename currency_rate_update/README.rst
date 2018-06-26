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

Currency Rate Update
====================

Import exchange rates from the Internet.

The module is able to use the following sources:

1. Admin.ch
   Updated daily, source in CHF.

2. European Central Bank (ported by Grzegorz Grzelak - OpenGLOBE.pl)
   The reference rates are based on the regular daily query
   procedure between central banks within and outside the European
   System of Central Banks, which normally takes place at 2.15 p.m.
   (14:15) ECB time. Source in EUR.
   http://www.ecb.europa.eu/stats/exchange/eurofxref/html/index.en.html

3. Yahoo Finance
   Updated daily

4. Polish National Bank (Narodowy Bank Polski) (by Grzegorz Grzelak - OpenGLOBE.pl)
   Takes official rates from www.nbp.pl. Adds rate table symbol in log.
   You should check when rates should apply to bookkeeping.
   If next day you should change the update hour in schedule settings
   because in Odoo they apply from date of update (date - no hours).

5. Banxico for USD & MXN (created by Agustín Cruz)
   Updated daily

6. Bank of Canada
   (WARNING: Currently not working)

7. National Bank of Romania (Banca Nationala a Romaniei)

Installation
------------





Configuration
-------------






The update can be set under the company form.
You can set for each services which currency you want to update.
The logs of the update are visible under the service note.
You can active or deactivate the update.
The module uses internal ir-cron feature from Odoo, so the job is
launched once the server starts if the 'first execute date' is before
the current day.

Usage
-----






=====

The module supports multi-company currency in two ways:

* when currencies are shared, you can set currency update only on one
  company
* when currencies are separated, you can set currency on every company
  separately

A function field lets you know your currency configuration.

If in multi-company mode, the base currency will be the first company's
currency found in database.

Know issues / Roadmap

To fix:
* Bank of Canada

Roadmap:
* Google Finance.
* Updated daily from Citibank N.A., source in EUR. Information may be delayed.
  This is parsed from an HTML page, so it may be broken at anytime.


Known issues / Roadmap
----------------------





Bug Tracker
-----------






Bugs are tracked on `GitHub Issues <https://github.com/OCA/account-financial-tools/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed feedback.


Credits
-------











### Contributors






* Nicolas Bessi <nicolas.bessi@camptocamp.com>
* Jean-Baptiste Aubort <jean-baptiste.aubort@camptocamp.com>
* Joël Grand-Guillaume <joel.grandguillaume@camptocamp.com>
* Grzegorz Grzelak <grzegorz.grzelak@openglobe.pl> (ECB, NBP)
* Vincent Renaville <vincent.renaville@camptocamp.com>
* Yannick Vaucher <yannick.vaucher@camptocamp.com>
* Guewen Baconnier <guewen.baconnier@camptocamp.com>
* Lorenzo Battistini <lorenzo.battistini@agilebg.com> (Port to V7)
* Agustin Cruz <openpyme.mx> (BdM)
* Jacque-Etienne Baudoux <je@bcim.be>
* Juan Jose Scarafia <jjscarafia@paintballrosario.com.ar>
* Mathieu Benoi <mathben963@gmail.com>
* Fekete Mihai <feketemihai@gmail.com> (Port to V8)
* Dorin Hongu <dhongu@gmail.com> (BNR)
* Paul McDermott
* Alexis de Lattre <alexis@via.ecp.fr>
* Miku Laitinen
* Assem Bayahi
* Daniel Dico <ddico@oerp.ca> (BOC)
* Dmytro Katyukha <firemage.dima@gmail.com>


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
