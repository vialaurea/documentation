Reverse Charges
===============

Reverse VAT
-----------

Introduction
------------

- Reverse VAT is a tax applied to VAT payers where the buyer, not the seller, pays the VAT to the state budget. Usually, the seller is responsible for the VAT by adding a certain tax amount to the final price.
- This type of VAT is also applicable in cases such as:
  1. When construction work is performed.
  2. When improving the condition of a building or structure.
  3. When taking over ownership of property.
  4. When purchasing mobile phones, tablets, laptops, or other computers, hard drives, etc.
  5. When buying wood.
  6. When buying ferrous or non-ferrous metals.

Installation and Configuration
------------------------------

- In the Odoo business management system, you need to install Account Invoice Reversed Tax Show.
- Before using this module, you need to perform the following configurations:
  - Create a new tax group for reverse taxes and assign them (important!).
  - Set the reverse tax field to Force calculate the invoice.
  - Do not use the checkbox for other types of taxes.

  .. image:: reverse_charges/img1.jpg
      :alt: Tax group configuration

Daily Use Scenarios
-------------------

- When selling an item subject to reverse VAT, you need to manually change the tax.

  .. image:: reverse_charges/img2.jpg
      :alt: Manually change the tax

  If configured correctly, the VAT amount is automatically calculated in the final calculation.

  .. image:: reverse_charges/img3.jpg
      :alt: Automatic VAT calculation

Integrations and Connections with Other Modules
-----------------------------------------------

- The module only works with the Accounting module.