Acceptance-transfer act
===================

Introduction
------------

**Low-value tangible assets** are assets whose acquisition value is lower than the selected minimum acquisition value for fixed assets. Assets below this value are classified as inventory. When such assets are acquired and put into use, they are immediately written off as expenses for accounting purposes. However, companies strive to account for low-value assets, track their movements and condition.

When using the Odoo system, it is recommended to account for low-value tangible assets in the standard Maintenance module.

Installation and Configuration
-------------------

- The l10n_lt_equipment_transfer_act module is installed along with the standard Maintenance module.

- No additional configuration is required.

Daily Use Scenarios
-------------------

- Using standard Odoo functionality, go to Maintenance >> Equipment to enter one or more records and assign them to a selected employee.

  .. image:: transfer_act/image01.jpg

- After entering the data, select the print function.

  .. image:: transfer_act/image02.jpg

- You can print both from the equipment record and from the equipment list. If we print from the list, we can select not just one, but several units of various assets (both low-value and long-term), and they will be included in a common printed acceptance-transfer act.

  .. image:: transfer_act/image03.jpg

Reports and Documentation
-------------------

When selecting the Print >> Equipment Transfer Act button, a launch parameter opens where you need to fill in:

  .. image:: transfer_act/image04.jpg

- **Transferred by** - select from the employee list the responsible employee who transfers the assets;
- **Received by** - select from the employee list the responsible employee to whom the assets are being transferred;
- **Date** - enter the date. By default, it is always filled with today's date.

When you click 'Print Act', a .pdf document of this format is generated:

  .. image:: transfer_act/image05.jpg

The document can be printed and submitted to responsible employees for signing.

Updates and Version Management
-------------------

The module is updated with each new Odoo version.