Mass accounting records management
==================================

Introduction
------------

- The technical name of the module is `mass_accounting_records_management`. The module is associated with the Accounting module but is not related to the LT localization. It can operate in any localization.
- The module is intended for consultants or highly experienced Odoo users when there is a need to manage GL entries in bulk.

Installation and Configuration
------------------------------

- **Module Installation**: Install the `mass_accounting_records_management` module.
- **Configuration**: No additional configuration is required.

Main Functions
--------------

- The module adds 2 additional Action buttons in Accounting >> Accounting >> GL Entries: **Cancel** and **Reset to Draft**.
- The Action buttons **Confirm** and **Delete** are part of the standard Accounting module.

  .. image:: mass_accounting_records_management/image01.jpg

- Step-by-step instructions on how to use these functions.

Daily Use Scenarios
-------------------

- The module is useful, for example, when managing fixed asset entries where many GL entries are created for past periods upon asset confirmation, and later, they need to be removed or corrected due to errors.

  .. image:: mass_accounting_records_management/image02.jpg

Updates and Version Control
----------------------------

- **Warning**: In version 16, the module violates an Odoo rule where it is prohibited to cancel GL entries for certain invoices. With this module, it is possible to cancel invoices.
- The module can be freely used in version 15.
