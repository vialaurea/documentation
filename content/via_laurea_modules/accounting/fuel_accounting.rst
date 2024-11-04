Fuel Registration by Car
========================

1. Introduction
----------------

This module is designed to manage vehicle fleets, conduct fuel accounting, and monitor and analyze other expenses related to vehicles. 
It contributes to compliance with Lithuanian accounting standards in the Odoo system.

2. Installation and Configuration
----------------------------------

Before using this module, specific settings need to be configured.

Go to "Vehicle Park" -> Configuration -> Settings:

.. image:: fuel_accounting/number1.jpg
   :alt: Configuration settings window

Configuration fields open:

.. image:: fuel_accounting/number2.jpg
   :alt: Vehicle card creation interface

- Specify the debit/credit fuel account.
- Choose the fuel products.
- Fuel journal: Either use the standard "various operations" or create a specialized one specifically for fuel accounting (for how to create a journal, see the "Starting with Odoo" instructions).

1. Main Features
----------------

Create a vehicle card and enter all necessary information:

- Click "New":

.. image:: fuel_accounting/number3.jpg
   :alt: Vehicle card creation interface

- Select a template (vehicle make) from the provided list.
- Enter the registration number.
- If needed, input information about the driver.
- Fill in the relevant fields about the vehicle.
- Fill in the required information in the tax information field.
- Specify the debit/credit account for fuel accounting.
- After filling in the tax information, we go to the templates:

.. image:: fuel_accounting/number4.jpg
   :alt: Additional vehicle information fields

Proceed to input additional vehicle details.

Once the vehicle card is completed and filled out, it is possible to register operations related to the specific vehicle.

When registering invoices, the necessary vehicle is assigned in the lines:

.. image:: fuel_accounting/number5.jpg
   :alt: Assigning vehicles in invoice registration

If services related to the vehicle were purchased, the information is displayed here on the vehicle card:

.. image:: fuel_accounting/number6.jpg
   :alt: Services related information display on vehicle card

Clicking on this button opens a window with all invoices.

When purchasing fuel:

.. image:: fuel_accounting/number7.jpg
   :alt: Fuel history window

Clicking this button opens a window with the entire fuel history:

.. image:: fuel_accounting/number8.jpg
   :alt: Fuel write-off interface

In the opened window, the purchased quantity, write-offs, and remaining fuel balance are displayed.

Fuel write-off is performed on the vehicle card by clicking the button:

.. image:: fuel_accounting/number9.jpg
   :alt: Details of fuel write-off

A window opens:

.. image:: fuel_accounting/number10.jpg
   :alt: Accessing the fuel journal

- Select a vehicle.
- Specify the date for the fuel write-off.
- Enter the amount of fuel to be written off.
- Click "Write off".

After forming the fuel write-off record, go to the "Fuel Journal":

.. image:: fuel_accounting/number11.jpg
   :alt: Checking draft entries

Here, draft entries are created, which need to be registered to ensure that the data and figures are recorded in the general ledger:

.. image:: fuel_accounting/number12.jpg
   :alt: Finalizing entries in the fuel journal

Before registering, by clicking on the desired line, you can check the correspondence that will register:

.. image:: fuel_accounting/number13.jpg
   :alt: Document management and archiving instructions

If everything is correct, return to the Fuel Journals, mark the entry you want to register, and click Action -> Post Entries.

.. image:: fuel_accounting/number14.jpg
   :alt: Integration with other modules

1. Reports and Documentation
-----------------------------

A fuel write-off report can be printed in the fuel accounting module.

- In the vehicle card, click "Print"
- Select "fuel write-off report"
- In the opened window, select the date for which the report should be printed and choose the format: