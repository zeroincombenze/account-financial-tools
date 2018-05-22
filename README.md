[![Build Status](https://travis-ci.org/zeroincombenze/account-financial-tools.svg?branch=9.0)](https://travis-ci.org/zeroincombenze/account-financial-tools)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/account-financial-tools/badge.svg?branch=9.0)](https://coveralls.io/github/zeroincombenze/account-financial-tools?branch=9.0)
[![codecov](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/9.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/9.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-9.svg)](https://github.com/OCA/account-financial-tools/tree/9.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-9.svg)](http://wiki.zeroincombenze.org/en/Odoo/9.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-9.svg)](http://wiki.zeroincombenze.org/en/Odoo/9.0/man/FI)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-9.svg)](http://erp9.zeroincombenze.it)


























































[![en](http://www.shs-av.com/wp-content/en_US.png)](http://wiki.zeroincombenze.org/it/Odoo/7.0/man)

Account financial Tools for Odoo/Odoo
=====================================

This project aims to make the accounting usage system easy and painless.
It provides addons to:

 - Update the currency rate automatically via web services
 - Push credit management and follow up to next level
 - Generate reversed account moves
 - Cancel invoices with ease
 - Force draft accounting by default
 - Enforce partners on account moves

And much more.

[//]: # (addons)


Available addons
----------------
addon | version | OCA version | summary
--- | --- | --- | ---
[account_fiscal_position_vat_check](account_fiscal_position_vat_check/) | 9.0.1.0.0 | :repeat: | Check VAT on invoice validation
[account_fiscal_year](account_fiscal_year/) | 9.0.1.0.0 | :repeat: | Account Fiscal Year
[account_invoice_currency](account_invoice_currency/) | 9.0.1.0.0 | :repeat: | Company currency in invoices
[account_move_locking](account_move_locking/) | 9.0.1.0.0 | :repeat: | Move locked to prevent modification
[account_permanent_lock_move](account_permanent_lock_move/) | 9.0.1.0.0 | :repeat: | Permanent Lock Move
[account_renumber](account_renumber/) | 9.0.1.0.0 | 9.0.1.0.1 | Account Renumber Wizard
[account_reversal](account_reversal/) | 9.0.1.0.0 | :repeat: | Wizard for creating a reversal account move
[currency_rate_update](currency_rate_update/) | 9.0.1.0.0 | :repeat: | Currency Rate Update


Unported addons
---------------
addon | version | OCA version | summary
--- | --- | --- | ---
[account_asset_management](account_asset_management/) | 8.0.2.6.0 (unported) | :repeat: | Assets Management
[account_asset_management_xls](account_asset_management_xls/) | 8.0.0.1.0 (unported) | :repeat: | Assets Management Excel reporting
[account_auto_fy_sequence](account_auto_fy_sequence/) | 8.0.0.1.0 (unported) | :x: | Automatic Fiscal Year Sequences
[account_balance_line](account_balance_line/) | 8.0.1.1.0 (unported) | 9.0.1.1.0 | Display balance totals in move line view
[account_cancel_invoice_check_payment_order](account_cancel_invoice_check_payment_order/) | 1.0 (unported) | :repeat: | Cancel invoice, check on payment order
[account_cancel_invoice_check_voucher](account_cancel_invoice_check_voucher/) | 1.0 (unported) | :repeat: | Cancel invoice, check on bank statement
[account_chart_update](account_chart_update/) | 8.0.1.2.0 (unported) | 9.0.1.0.0 | Detect changes and update the Account Chart from a template
[account_check_deposit](account_check_deposit/) | 8.0.0.1.0 (unported) | 9.0.0.1.0 | Manage deposit of checks to the bank
[account_constraints](account_constraints/) | 8.0.1.1.0 (unported) | :repeat: | Account Constraints
[account_credit_control](account_credit_control/) | 8.0.0.3.0 (unported) | 9.0.1.0.3 | Account Credit Control
[account_credit_control_dunning_fees](account_credit_control_dunning_fees/) | 8.0.0.1.0 (unported) | :repeat: | Credit control dunning fees
[account_default_draft_move](account_default_draft_move/) | 8.0.1.0.0 (unported) | :repeat: | Move in draft state by default
[account_invoice_constraint_chronology](account_invoice_constraint_chronology/) | 8.0.1.0.0 (unported) | :repeat: | Account Invoice Constraint Chronology
[account_invoice_tax_required](account_invoice_tax_required/) | 8.0.1.0.0 (unported) | 9.0.1.0.0 | Tax required in invoice
[account_journal_always_check_date](account_journal_always_check_date/) | 8.0.0.1.0 (unported) | :repeat: | Option Check Date in Period always active on journals
[account_journal_period_close](account_journal_period_close/) | 8.0.1.0.0 (unported) | :repeat: | Account Journal Period Close
[account_move_batch_validate](account_move_batch_validate/) | 8.0.0.2.0 (unported) | :repeat: | Account Move Batch Validate
[account_move_line_no_default_search](account_move_line_no_default_search/) | 8.0.0.1.0 (unported) | :repeat: | Move line search view - disable defaults for period and journal
[account_move_line_payable_receivable_filter](account_move_line_payable_receivable_filter/) | 8.0.1.0.0 (unported) | :repeat: | Filter your Journal Items per payable and receivable account
[account_move_line_search_extension](account_move_line_search_extension/) | 8.0.0.6.0 (unported) | :repeat: | Journal Items Search Extension
[account_move_template](account_move_template/) | 8.0.1.0.0 (unported) | :repeat: | Templates for recurring Journal Entries
[account_partner_required](account_partner_required/) | 8.0.0.1.0 (unported) | :repeat: | Account partner required
[account_reset_chart](account_reset_chart/) | 8.0.1.0.0 (unported) | :repeat: | Delete the accounting setup from an otherwise reusable database
[account_tax_analysis](account_tax_analysis/) | 8.0.1.0.0 (unported) | :repeat: | Tax analysis
[account_tax_chart_interval](account_tax_chart_interval/) | 8.0.1.0.0 (unported) | :repeat: | Tax chart for a period interval
[account_tax_update](account_tax_update/) | 1.0.44 (unported) | 9.0.1.0.45 (unported) | Update tax wizard
[async_move_line_importer](async_move_line_importer/) | 0.1.2 (unported) | :repeat: | Asynchronous move/move line CSV importer
[currency_rate_date_check](currency_rate_date_check/) | 8.0.1.0.0 (unported) | :repeat: | Make sure currency rates used are always up-to-update

[//]: # (end addons)

Translation Status
[![Transifex Status](https://www.transifex.com/projects/p/OCA-account-financial-tools-9-0/chart/image_png)](https://www.transifex.com/projects/p/OCA-account-financial-tools-9-0)

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

[![chat with us](https://www.shs-av.com/wp-content/chat_with_us.gif)](https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b)
