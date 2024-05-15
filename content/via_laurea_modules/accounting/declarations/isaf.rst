​iSAF
====

Introduction
------------

- Since 2019-07-01, all legal entities that are VAT payers must submit the data of issued and received VAT invoice registers to VMI monthly by the 20th day of the following month. The register is called the iSAF declaration. The rules for filling in and submitting VAT invoice registers are approved by the VMI Order No. VA-55 dated 2004-04-21 "On the management of VAT invoice registers".

Installation and Configuration
-------------------------------

- Install the module (technical name) - l10n_lt_isaf
- For configuration, you need to set the VAT classifier codes approved by the State Tax Inspectorate (VMI):
  Select the main menu - Accounting -> Configuration -> Taxes

  .. image:: isaf/img01.jpg
      :alt: Main menu - Accounting -> Configuration -> Taxes

- In the tax environment, the Tax code is mandatory

  .. image:: isaf/img02.jpg
      :alt: Mandatory Tax Code

Main Functions
--------------

- The main function of the iSAF report is the cross-checking (clients/suppliers) of the data of registered invoices (issued and received) in the VMI information system

Reports and Documentation
-------------------------

Before generating iSAF, data verification is recommended.
Main menu - Reports -> Invoice registers

  .. image:: isaf/img03.jpg
      :alt: Main menu - Reports -> Invoice registers

The reporting period date (month), purchases/sales are shown separately, and VAT information is also highlighted

  .. image:: isaf/img04.jpg
      :alt: Reporting period date - purchases/sales and VAT information

The generated report shows ALL and non-declared data

  .. image:: isaf/img05.jpg
      :alt: Generated report showing all and non-declared data

iSAF Generation
---------------

Main menu - i.MAS -> i.SAF to create a new report

  .. image:: isaf/img06.jpg
      :alt: Main menu - i.MAS -> i.SAF new report

The reporting period (month), the type of register (registered invoices) can be selected, by report (all, supplier or invoices)

  .. image:: isaf/img07.jpg
      :alt: Reporting period and register type selection

For example: Register type - All -> (save button) -> Automatically collect invoices

  .. image:: isaf/img08.jpg
      :alt: Automatically collect invoices

Automatically generated invoice register to be formed into an XML file

  .. image:: isaf/img09.jpg
      :alt: Form into XML file

Download the generated report

  .. image:: isaf/img10.jpg
      :alt: Download report

and send

  .. image:: isaf/img11.jpg
      :alt: Send report

  .. image:: isaf/img12.jpg
      :alt: Report sent

Integrations and Connections with Other Modules
-----------------------------------------------

- How this module integrates with other Odoo modules or external systems.
- Special integration instructions, if needed.