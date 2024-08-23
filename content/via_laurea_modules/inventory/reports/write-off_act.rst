Write-off Act
=============

Introduction
------------

- Extension of the standard Odoo functionality for scrapping: the ability to print a scrap report.
- This module contributes to compliance with Lithuanian accounting standards in the Odoo system, if applicable.

Installation and Configuration
------------------------------

- **Installation Instructions**: The module `Inventory scrap report` (technical name `inventory_scrap_report`) must be installed along with the standard Odoo Inventory module (technical name `stock`).
- **Initial Configuration**: No additional configuration is required.

Daily Use Scenarios
-------------------

- Using the standard Odoo functionality, navigate to Inventory -> Operations -> Scrap. Enter one or more product scraps from the warehouse.

  .. image:: write-off_act/image01.jpg

Reports and Documentation
-------------------------

- After entering the document, it is possible to print the scrap report.

  .. image:: write-off_act/image02.jpg

- In the window that opens, the following fields need to be filled in:
  - **Scrap Report Date**: Select the date.
  - **Scrap Report Number**: Manually enter the number (there is no automatic numbering).
  - **Scrap Basis, Commission Established, Commission Suggests**: Texts that will appear in the report; not mandatory to fill in.
  - **Commission Chairman, Commission Members, Materially Responsible Person, and Accounting Staff**: Select from the list of employees.

  .. image:: write-off_act/image03.jpg

- Press "Print" to generate the following document:

  .. image:: write-off_act/image04.jpg

- If needed, the scrap report can also be printed from the list view in the standard way.

Updates and Version Control
----------------------------

- The module is updated with each new version of Odoo.
