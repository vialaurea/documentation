Intrastat
=========

Installation and Configuration
------------------------------

1. Install the modules ``account_intrastat`` and ``l10n_lt_intrastat``.

2. After installing the modules, two additional menus appear in the Accounting module:

   - **Accounting >> Reports >> Intrastat Report**
   - **Accounting >> Configuration >> Intrastat Code**

   .. image:: intrastat/Image01.jpg

   The Intrastat Code parameter includes all the primary classifiers from the Lithuanian Customs: transaction codes, delivery condition codes, Lithuanian counties classifier, and Combined Nomenclature (KN).

3. In the Combined Nomenclature parameter, you must add Lithuanian translations only for those KN codes that your company uses for sales/purchases within the EU. Other codes can be left blank.

   .. image:: intrastat/Image02.jpg

   If required by the Lithuanian Customs Combined Nomenclature (KN) classifier, you must also fill in the unit of measure field.

4. The **Accounting >> Configuration >> Incoterm** contains standard Incoterm conditions. These are linked to the accounting module and are installed even without the Intrastat module.

   .. image:: intrastat/Image03.jpg

5. In the main settings of the Accounting module (**Accounting >> Configuration >> Settings**), you can set the default Incoterm conditions and transaction types.

   .. image:: intrastat/Image04.jpg

6. In this parameter, you can also set the Intrastat-required county code of the company if the entire company is in one location, within one Lithuanian county. If part of the company (e.g., a warehouse) is in another Lithuanian county or the company has multiple branches (Vilnius, Kaunas, Klaipėda, Šiauliai...) with separate warehouses, the county code is set for each warehouse separately under **Inventory >> Configuration >> Warehouses**.

   .. image:: intrastat/Image05.jpg


Main Functions
--------------

1. In the product form, the Combined Nomenclature (KN) code must be set, selected from the Intrastat code classifier, along with the country of origin, chosen from the standard Odoo country classifier. If there is an additional unit of measure, you need to enter the product unit equivalent with the units used in the declaration.

   .. image:: intrastat/Image06.jpg

2. The standard weight field must also be filled in on the product form.

3. When entering a Customer or Vendor invoice, you must fill in the transport type in each invoice, selecting it from the Intrastat code classifier.

   .. image:: intrastat/Image07.jpg

4. The Intrastat country is filled in automatically if set in the Contact form. The Incoterm conditions are also filled in automatically if set in parameter 5, but they can be manually adjusted even if the invoice is not canceled.

5. In the invoice lines (if not visible, it can be enabled through the "curtain" icon), you can enter the transaction type if it does not match the default setting in parameter 5, and the country of origin if it does not match the product form or is not specified in the product form.

   .. image:: intrastat/Image08.jpg


Reports and Documentation
--------------------------

1. Go to **Accounting >> Reports >> Intrastat Report**. By default, the report is always generated with data from the previous period, but there is a filter where you can select the current period, the previous period, or a custom date range.

   .. image:: intrastat/Image09.jpg

2. In the report, you can choose to include only export or import documents if the Lithuanian Customs, based on the previous calendar year's trade data with the EU, has instructed the company to submit only one type of report.

   .. image:: intrastat/Image10.jpg

3. If needed, for example, when there are many lines, the report data can be exported to `.xls` or printed in `.pdf`.

4. Once the report is fully completed and reviewed, you can click the button to generate an XML document for the Lithuanian Customs declaration.

   .. image:: intrastat/Image11.jpg

5. In the launch parameters, you need to select the year, month (by default, it always offers the previous period), the type of Intrastat, i.e., whether the declaration is for exported goods or imported goods, and the action - primary, corrected, or zero.

   .. image:: intrastat/Image12.jpg

6. It is mandatory to select the responsible company employee in the **Contact Person** field from the contact list, as this data is required for the Lithuanian Customs report.

   .. image:: intrastat/Image13.jpg

7. The contact must have a phone number and job title filled in, as these details are included in the report's XML document, so that Lithuanian Customs officials can contact the responsible employee if necessary.


Daily Use Scenarios
-------------------

1. If the report is not fully completed, a yellow informational message will appear, indicating potential discrepancies: missing product weights, missing KN codes, missing transaction codes, etc.

   .. image:: intrastat/Image14.jpg

2. To correct errors, simply click on the highlighted text in the yellow line. For example, if the message indicates that some products do not have KN codes, a list of those products will open, allowing you to immediately enter the missing data from the list.

   .. image:: intrastat/Image15.jpg

3. Similarly, if the message indicates that "Transaction codes are missing in some lines," a different type of window will open, showing which invoice lines have missing transaction codes, and allowing you to fill them in immediately.

   .. image:: intrastat/Image16.jpg

4. It is also possible to correct product weights or additional units of measure used for the declaration.

5. After entering the data, it is recommended to regenerate the report or reload it.

   .. image:: intrastat/Image17.jpg

6. The transport types must be checked manually. In the invoice list, you can use a filter or group by transport type.

   .. image:: intrastat/Image18.jpg

7. If you ignore the errors and attempt to generate the XML document for the Lithuanian Customs declaration, the system will also check whether all the required information is filled in during the document generation process and will not allow the document to be created until the errors are corrected. A message will be displayed indicating which errors need to be corrected and where.

   .. image:: intrastat/Image19.jpg

8. If the error message is large and difficult to remember, you can copy it.

9. Only after correcting the errors will it allow you to generate the XML document, which can then be uploaded to the Lithuanian Customs electronic declaration system.


Updates and Version Control
----------------------------

- This guide is intended for Intrastat reports for Odoo Enterprise versions 16 and 17.
- Some parameters and functionality may not be available if you generate a report in another version.
