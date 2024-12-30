CMR
===

1. Introduction
----------------
- This is a report under the Convention on the Contract for the International Carriage of Goods by Road (CMR) for the carriage of goods by land.
- The module contributes to compliance with the international transportation system by printing international freight bills of lading.

2. Installation and Configuration
----------------------------------
- The CMR is printed from the Inventory module, so this module must be installed.
- Check whether the CMR report module, technically named stock_cmr_report, is installed. Additionally, check whether the Intrastat module is installed and configured.
- No additional settings are required for the initial configuration. 

However, before generating the report, it is necessary to properly enter the product card(s): the weight, Intrastat KN code (for more information, see the Intrastat declaration documentation) and country of origin of each product must be entered.

3. Main Features
-----------------
In the module Inventory -> Operations -> Transfers >> select the required unloading (OUT) document. The document must be in the "Ready" or "Completed" status, then select Print -> CMR..

  .. image:: cmr/image01.jpg


4. Reports and Documentation
-----------------------------
Some of the CMR report lines are filled in automatically, while others must be filled in manually.

Automatically filled in:

- **Template languages** - by default, En/Lt is offered, but you can choose Lt/En and Ru/En
- **4. Cargo loading location** - taken from Inventory -> configuration -> warehouses, the specific warehouse address specified in the parameter
- **4. Country** - taken from Inventory -> configuration -> warehouses, the specific warehouse address specified in the parameter
- **4. Date** - from the loading document
- **5. Attached documents** - if an invoice is issued from the sales order, then its number is filled in automatically, if the invoice has not been created, enter the number manually
- **9. Cargo name** and **10. Statistical number** are filled in from the product card Accounting -> KN code. This field is related to the Intrastat report (see Intrastat report)
- **11. Gross weight, kg** - the weight of the shipment is taken from the document from which the CMR report is printed, additional information on the card, field shipment weight
- **21. Place of collection** - taken from Inventory -> configuration -> warehouses, the specific warehouse address specified in the parameter
- **22. Date of collection** - by default, today's date is entered

If necessary, all fields can be adjusted manually. The remaining fields can be filled in manually.

  .. image:: cmr/image02.jpg

The report can be formatted in XLSX format using Generate CMR or PDF - Generate CMR (PDF). If needed, it can also be printed from the list of shipping documents (OUT) in the standard way, but it is necessary to select shipping documents (OUT) from the same partner only.

5. Integrations and Connectivity with Other Modules
----------------------------------------------------
- The module is linked to the standard Intrastat module (see more in the Intrastat declaration documentation).

6. Updates and Version Control
-------------------------------
- The module is updated with each new version of Odoo.
