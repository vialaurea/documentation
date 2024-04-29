Fuel Registration by Car
========================

Introduction
------------

This module is designed to manage the vehicle fleet, maintain fuel accounting, and monitor and analyze other expenses related to vehicles.
How the module contributes to compliance with Lithuanian accounting standards in the Odoo system.

Installation and Configuration
-------------------------------

**Installation Instructions**: Steps required for module installation.

**Initial Configuration**: Before starting to use this module, settings are required. Navigate to "Vehicle Fleet" -> "Configuration" -> "Settings":

.. image:: _static/your_image_path_here.jpg
   :alt: Settings Fields

Specify the fuel debit/credit account.
Select fuel products.
Fuel journal: You can use the standard "miscellaneous operations" or create a separate one specifically related to fuel accounting (for creating a journal, see the instruction "Getting Started with Odoo").

Main Features
-------------

Create a vehicle card and enter all the necessary information:
Click New

- Select a template (vehicle brand) from the list provided;
- Enter the registration number;
- If necessary, enter information about the driver;
- Fill in the relevant fields about the vehicle;
- In the tax information field, fill in the required information;
- Specify the fuel accounting debit/credit account;
- After filling in the tax information, move on to templates:

Further fill in the information about the vehicle.
Having created and filled in the information on the vehicle card, it is possible to register operations related to a specific vehicle.
When registering invoices, the necessary vehicle is assigned in the lines:

If these were services purchased related to the vehicle, the information in the vehicle card is visible here:

Upon clicking this button, a window opens with all the invoices.

If fuel was purchased:

Clicking this button opens a window with the entire fuel history:

In the opened window, the purchased quantity, write-offs, and fuel balance are visible.
Fuel write-off is performed in the vehicle card by pressing the button

A window opens:

- Select a vehicle;
- Specify the date for which the fuel write-off is being made;
- Enter the amount of fuel being written off.
- Click "Write-off".
After forming the fuel write-off entry, go to "Fuel Journal":

Here, draft entries are created, which need to be registered to ensure that the data and figures are registered in the general ledger:

Before registering, by clicking on the desired row, we can check what correspondence will register:

If everything is correct, go back to the Fuel Journals, mark the entry you want to register with a checkmark, and click Action -> Post entries:

Reports and Documentation
-------------------------

How to generate reports using the module.
Instructions for document management and archiving.

Integrations and Relationships with Other Modules
--------------------------------------------------

How this module integrates with other Odoo modules or external systems.
Special integration instructions if needed.

Troubleshooting and FAQ
------------------------

Common problems and their solutions.
Answers to frequently asked questions about this module.

Updates and Version Management
------------------------------

How to update the module.
Version management practices.

Appendices
----------

Screenshots and visual instructions.
Useful links and additional resources.
