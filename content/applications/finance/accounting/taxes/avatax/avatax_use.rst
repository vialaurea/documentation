==========
AvaTax use
==========

AvaTax is a tax calculation software that can be integrated with Odoo in the United States and
Canada. Once the :doc:`integration setup <../avatax>` is complete, the calculated tax is simple and
automatic.

Tax calculation
===============

Automatically calculate taxes on Odoo quotations and invoices with AvaTax by confirming the
documents during the sales flow. Alternatively, calculate the taxes manually by clicking the
:guilabel:`Compute taxes using Avatax` button while these documents are in draft mode.

.. tip::
   Clicking the :guilabel:`Compute taxes using Avatax` button recalculates taxes if any product
   lines are edited on the invoice.

.. image:: avatax_use/calculate-avatax.png
   :align: center
   :alt: Sales quotation with the confirm and compute taxes using AvaTax buttons highlighted.

The tax calculation is triggered during the following :ref:`automatic trigger
<avatax/automatic-triggers>` and :ref:`manual trigger <avatax/manual-triggers>` circumstances.

.. _avatax/automatic-triggers:

Automatic triggers
------------------

- When the sales rep sends the quote by email with :guilabel:`Send by email` button (pop-up).
- When the customer views the online quote on the portal.
- When a quote is confirmed and becomes a sales order.
- When the customer views the invoice on the portal.
- When a draft invoice is validated.
- When the customer views the subscription in the portal.
- When a subscription generates an invoice.
- When the customer gets to the last screen of the eCommerce checkout.

.. _avatax/manual-triggers:

Manual triggers
---------------

- :guilabel:`Compute taxes using Avatax` button at the bottom of the quote.
- :guilabel:`Compute taxes using Avatax` button at the top of the invoice.

.. tip::
   Use the :guilabel:`Avalara Partner Code` field that is available on customer records, quotations,
   and invoices to cross-reference data in Odoo and AvaTax. This field is located under the
   :menuselection:`Other info` tab of the sales order or quotation in the :guilabel:`Sales` section.

   On the customer record, navigate to *Contacts app* and select a contact. Then open the
   :guilabel:`Sales & Purchase` tab and the :guilabel:`Avalara Partner Code` under the
   :guilabel:`Sales` section.

.. important::
   The :guilabel:`Automatic Tax Mapping (AvaTax)` fiscal position is also applied on those Odoo
   documents, like subscriptions.

.. seealso::
   - :doc:`../fiscal_positions`

AvaTax synchronization
======================

Synchronization occurs with AvaTax, when the *invoice* is created in Odoo. This means the sales tax
is recorded with Avalara (AvaTax software developer).

To do so, navigate to :menuselection:`Sales app --> Orders --> Quotations`. Select a quotation from
the list.

After confirming a quotation and validating the delivery, click :guilabel:`Create Invoice`. Indicate
whether it is a :guilabel:`Regular invoice`, :guilabel:`Down payment (percentage)`, or
:guilabel:`Down payment (fixed amount)`.

Then click :guilabel:`Create and view invoice`. The recorded taxes can be seen in the
:guilabel:`Journal Items` tab of the invoice. There will be different taxes depending on the
location of the :guilabel:`Delivery Address`.

.. image:: avatax_use/journal-items.png
   :align: center
   :alt: Journal items highlighted on a invoice in Odoo.

Finally, press the :guilabel:`Confirm` button to complete the invoice and synchronize with the
AvaTax portal.

.. warning::
   An invoice cannot be :guilabel:`Reset to draft` because this causes de-synchronization with the
   AvaTax Portal. Instead, click :guilabel:`Add credit note` and state: `Sync with AvaTax Portal`.
   See this documentation: :doc:`../../../accounting/customer_invoices/credit_notes`.

Fixed price discounts
=====================

Add a fixed price discount to a valuable customer by click :guilabel:`Add a line` on the customer's
invoice. Add the product discount and set the :guilabel:`Price` to either a positive or negative
value. To recalculate the taxes, click :guilabel:`Compute taxes using Avatax`.

.. tip::
   Tax calculation can even be done on negative subtotals and credit notes.
