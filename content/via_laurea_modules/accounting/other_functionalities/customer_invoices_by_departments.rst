Customer invoices by departments
================================

Introduction
------------

- Odoo standard allows creating multiple sales journals and numbering sales invoices differently. However, the journal in the sales invoice can only be selected manually by default.
- This module enables automatic numbering of sales invoices by the company's physical division. For example, if the company's activity is registered in Kaunas but also has branches in Vilnius, Klaipėda, and Šiauliai, it is possible to number sales invoices separately by branch, i.e., by sales team.
- The module allows different numbering of sales invoices following the STATE TAX INSPECTORATE UNDER THE MINISTRY OF FINANCE OF THE REPUBLIC OF LITHUANIA ORDER ON THE MANAGEMENT OF VAT INVOICE REGISTERS, allowing the numbering of invoices according to the company's internal procedures.

Installation and Configuration
------------------------------

- Install the module `customer_invoices_by_departments`.
- To configure the module:
  1. In the Accounting module, create separate journals, e.g., Kaunas division sales, Klaipėda sales division, etc. The journal type must be Sales, and the short code must be unique, as it will be used for invoice numbering.

  .. image:: customer_invoices_by_departments/img01.jpg
      :alt: Create separate journals

  2. In the Sales module >> Configuration >> Sales Teams or in the CRM module >> Configuration >> Sales Teams, create separate teams according to the company's physical divisions, e.g., Vilnius branch, Šiauliai branch, Alytus branch, etc.

  .. image:: customer_invoices_by_departments/img02.jpg
      :alt: Create sales teams

  3. Assign each sales team an appropriate sales journal and employees working in that division. It is RECOMMENDED to assign all employees (not just salespeople) to the appropriate sales teams.

  .. image:: customer_invoices_by_departments/img03.jpg
      :alt: Assign sales journal and employees

Main Functions
--------------

- The sales employee, logged into their account, creates new sales orders through the sales module. By default, when creating an SO, the sales team is filled in according to the employee's team assignment. When creating a new invoice from the SO, the sales journal assigned to the sales team is automatically selected in the invoice.

  .. image:: customer_invoices_by_departments/img04.jpg
      :alt: Sales team and journal assignment

Daily Use Scenarios
-------------------

- If the employee is not assigned to any sales team (division), when creating an SO and issuing (creating) an invoice, the first journal in order will be suggested by default, according to Odoo standard. The employee can select the required journal manually.

  .. image:: customer_invoices_by_departments/img05.jpg
      :alt: Default journal selection

- When issuing (creating) an invoice through Accounting >> Customers >> Invoices, the first journal in order will be suggested by default (according to Odoo standard), regardless of whether the employee is assigned to a sales team or not. When the sales team is selected manually in the invoice, the sales journal will be selected according to the sales team automatically. The employee can also select the required journal manually.

  .. image:: customer_invoices_by_departments/img06.jpg
      :alt: Manual sales team and journal selection

- If the employee is not assigned to any sales team (division), creating a new sales order will not automatically fill in the sales team. But if the employee selects the sales team manually, when issuing (creating) the sales invoice, the journal will be suggested according to the sales team from the sales order.

  .. image:: customer_invoices_by_departments/img07.jpg
      :alt: Manual sales team selection

- If the employee is assigned to one sales team (division) and manually selects another sales team when creating a new sales order, the sales journal will be assigned according to the sales team from the sales order (not according to the employee) when issuing (creating) the sales invoice.

  .. image:: customer_invoices_by_departments/img08.jpg
      :alt: Sales team selection based on sales order

- The same sales journal can be assigned to multiple sales teams, e.g., Klaipėda and Palanga sales teams issue invoices in the Klaipėda sales journal.

  .. image:: customer_invoices_by_departments/img09.jpg
      :alt: Assigning the same journal to multiple teams

Integrations and Connections with Other Modules
-----------------------------------------------

- Regardless of how invoices are numbered, all will be included in a single iSAF report (see more in the iSAF declaration submission documentation). It is not possible to submit a declaration for separate divisions.
- It is not possible to print the S/F register (see more in the S/F register documentation) by different divisions in the report. A single consolidated invoice register report for all divisions will be printed.
