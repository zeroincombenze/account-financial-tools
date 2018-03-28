[![Build Status](https://travis-ci.org/zeroincombenze/account-financial-tools.svg?branch=7.0)](https://travis-ci.org/zeroincombenze/account-financial-tools)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/account-financial-tools/badge.svg?branch=7.0)](https://coveralls.io/github/zeroincombenze/account-financial-tools?branch=7.0)
[![codecov](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/7.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/account-financial-tools/branch/7.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-7.svg)](https://github.com/OCA/account-financial-tools/tree/7.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-7.svg)](http://wiki.zeroincombenze.org/en/Odoo/7.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-7.svg)](http://wiki.zeroincombenze.org/en/Odoo/7.0/man/FI)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-7.svg)](http://erp7.zeroincombenze.it)



[![en](https://github.com/zeroincombenze/grymb/blob/master/flags/en_US.png)](https://www.facebook.com/groups/openerp.italia/)
================================================================================================
================================================================================================

Account financial Tools for Odoo
================================

This project aims to make the accounting usage system easy and painless.
It provides addons to:

 - Update the currency rate automatically via web services
 - Push credit management and follow up to next level
 - Generate reversed account moves
 - Cancel invoices with ease
 - Force draft accounting by default
 - Enforce partners on account moves

Translation Status
[![Transifex Status](https://www.transifex.com/projects/p/OCA-account-financial-tools-7-0/chart/image_png)](https://www.transifex.com/projects/p/OCA-account-financial-tools-7-0)

And much more.
And much more.

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


Available addons
----------------
addon | version | OCA version | summary
--- | --- | --- | ---
[account_asset_management](account_asset_management/) | 2.4 | :repeat: | Assets Management
[account_asset_management_xls](account_asset_management_xls/) | 0.1 | :repeat: | Assets Management Excel reporting
[account_auto_fy_sequence](account_auto_fy_sequence/) | 0.1 | :repeat: | Automatic Fiscal Year Sequences
[account_balance_line](account_balance_line/) | 1.1 | :repeat: | Display balance totals in move line view
[account_cancel_invoice_check_payment_order](account_cancel_invoice_check_payment_order/) | 1.0 | :repeat: | Cancel invoice, check on payment order
[account_cancel_invoice_check_voucher](account_cancel_invoice_check_voucher/) | 1.0 | :repeat: | Cancel invoice, check on bank statement
[account_chart_update](account_chart_update/) | 1.2 | :repeat: | Detect changes and update the Account Chart from a template
[account_check_deposit](account_check_deposit/) | 0.1 | :repeat: | Manage deposit of checks to the bank
[account_compute_tax_amount](account_compute_tax_amount/) | 1.0 | :repeat: | Recompute tax_amount
[account_constraints](account_constraints/) | 1.1 | :repeat: | Account Constraints
[account_credit_control](account_credit_control/) | 0.2.0 | :repeat: | Account Credit Control
[account_credit_control_dunning_fees](account_credit_control_dunning_fees/) | 0.1.0 | :repeat: | Credit control dunning fees
[account_default_draft_move](account_default_draft_move/) | 1.0 | :repeat: | Move in draft state by default
[account_fiscal_position_vat_check](account_fiscal_position_vat_check/) | 0.1 | :repeat: | Check VAT on invoice validation
[account_invoice_currency](account_invoice_currency/) | 1.0 | :repeat: | Company currency in invoices
[account_journal_always_check_date](account_journal_always_check_date/) | 0.1 | :repeat: | Option Check Date in Period always active on journals
[account_journal_entry_posted_async](account_journal_entry_posted_async/) | 0.1 | :repeat: | Automatically post account journal entries asynchronously
[account_journal_period_close](account_journal_period_close/) | 1.0 | :repeat: | Account Journal Period Close
[account_move_batch_validate](account_move_batch_validate/) | 0.2 | :repeat: | Account Move Batch Validate
[account_move_line_no_default_search](account_move_line_no_default_search/) | 0.1 | :repeat: | Move line search view - disable defaults for period and journal
[account_move_line_search_extension](account_move_line_search_extension/) | 0.1 | :repeat: | Journal Items Search Extension
[account_move_select_reconciliation](account_move_select_reconciliation/) | 0.1 | :repeat: | Account Move Select Reconciliation
[account_move_template](account_move_template/) | 0.1 | :repeat: | Templates for recurring Journal Entries
[account_move_validation_improvement](account_move_validation_improvement/) | 1.0 | :repeat: | Wizard to validate multiple moves
[account_partner_required](account_partner_required/) | 0.1 | :repeat: | Account partner required
[account_renumber](account_renumber/) | 1.0 | :repeat: | Account renumber wizard
[account_reversal](account_reversal/) | 1.0 | :repeat: | Account Reversal
[account_tax_analysis](account_tax_analysis/) | 1.0 | :repeat: | Tax analysis
[account_tax_update](account_tax_update/) | 7.0.1.0.45 | :repeat: | Update tax wizard
[async_move_line_importer](async_move_line_importer/) | 0.1.2 | :repeat: | Asynchronous move/move line CSV importer
[currency_rate_date_check](currency_rate_date_check/) | 1.0 | :repeat: | Make sure currency rates used are always up-to-update
[currency_rate_update](currency_rate_update/) | 0.8 | :repeat: | Currency Rate Update
[l10n_fr_siret](l10n_fr_siret/) | 1.1.1 | :repeat: | French company identity numbers SIRET/SIREN/NIC

[//]: # (end addons)

[![chat with us](https://www.shs-av.com/wp-content/chat_with_us.gif)](https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b)
