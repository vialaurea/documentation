Long-term Asset Report Instruction
==================================

Introduction
------------

- The module enhances Odoo's long-term asset functionality, allowing you to assign asset objects to employees, enter additional asset information, and print various reports.

Installation and Configuration
------------------------------

- Install the modules ``l10n_lt_account_asset`` and ``account_asset_enterprise_extended``.

Asset Assignment to an Employee
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Go to the Long-term Assets module.
- Select the asset you want to assign and open it for editing. The status of the asset (active, draft, or closed) does not matter.
- In the "Assigned to Employee" field, select the employee from the list. Save the changes.

  .. image:: fixed_assets_reports/image01.jpg

Additional Asset Information
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Go to the Long-term Assets module.
- Select the asset and open it for editing. The status of the asset (active, draft, or closed) does not matter.
- Enter the following additional information:
  - **Inventory Number**: Enter the inventory number of the asset.
  - **Supplier Invoice Reference**: Enter the reference to the related supplier invoice.
  - **Commissioning Date**: Select the date when the asset was commissioned.

  .. image:: fixed_assets_reports/image02.jpg

Main Features
-------------

- If an employee to whom the asset is assigned leaves the company or is assigned another asset, you should update the long-term asset record by removing or changing the "Assigned to Employee" field.

Reports
-------

- Via laurea has developed special long-term asset reports for the Lithuanian market, which can be found in the Accounting module under Accounting >> Reports >> Via laurea long-term asset reports.
- In the report window, you can choose from three different reports: Asset Card, Commissioning Act, and Write-off Act.

  .. image:: fixed_assets_reports/image03.jpg

Daily Use Scenarios
-------------------

Asset Card
~~~~~~~~~~

- To print an asset card, select the appropriate report, choose the specific asset from the list, and set the date for which the card will be generated.

  .. image:: fixed_assets_reports/image04.jpg

- Choose the format in which you want to generate the card. The system will generate an asset card with all the data related to the selected asset.

  .. image:: fixed_assets_reports/image05.jpg

- **Important**: You can select multiple assets, and the system will generate a combined file with asset cards for all selected items.

Commissioning Act
~~~~~~~~~~~~~~~~~

- The Commissioning Act is created when an asset starts being used in the company's operations. To print it, enter the act number, select the specific asset from the list, date, and order number in the opened window. Assign the materially responsible person. Select the commission chairman and members from the list.

  .. image:: fixed_assets_reports/image06.jpg

- After filling in all the fields, choose the document format you want to generate. The data related to the asset will be pulled into the printable document from the asset card.

  .. image:: fixed_assets_reports/image07.jpg

- **Important**: Similar to the previous form, if you select multiple assets, commissioning acts will be generated for all selected items at once.

Write-off Act
~~~~~~~~~~~~~

- The Write-off Act is used to generate a document for writing off an asset. Select the appropriate asset report from the list, enter the act number, document and decommissioning dates, and select the commission chairman and members. In the decommissioning and commission proposal fields, you can enter the necessary text that will be displayed in the document. Generate the document in the required format.

  .. image:: fixed_assets_reports/image08.jpg

- The appropriate document is generated:

  .. image:: fixed_assets_reports/image09.jpg
  .. image:: fixed_assets_reports/image10.jpg

- **Important**: If you select multiple assets in this form, a single document will be generated, and all the written-off items will be listed in the table in the appendix.

Updates and Version Control
----------------------------

- The module is updated with each new version of Odoo.