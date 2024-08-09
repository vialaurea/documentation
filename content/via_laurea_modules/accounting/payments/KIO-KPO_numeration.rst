KIO-KPO Numeration
==================

Introduction
------------

- A cash order (KIO and KPO) is an accounting document used to record cash being deposited into or withdrawn from the cash register. When depositing cash, the fact of cash receipt must be documented using a Cash Receipt Order (KPO). When performing the opposite financial operation - withdrawing cash from the register, a Cash Expense Order (KIO) is issued.

Installation and Configuration
------------------------------

- Install the module ``l10n_lt_kio_kpo_receipt``.

- Go to **Accounting >> Configuration >> Journals** and select the cash journal(s). The KIO and KPO sequence can only be set in a journal where the type is set to Cash. You can set separate sequences for KIO and KPO.

  .. image:: l10n_lt_kio_kpo_receipt/image01.jpg

- In the **KIO Sequence** field, select a sequence from the list or create a new one.

  .. image:: l10n_lt_kio_kpo_receipt/image02.jpg

  Fill in the required fields:
  
  - **Name**: The name of the sequence. This name is internal and is only displayed when selecting the sequence from the list.
  - **Prefix**: The prefix of the number, usually "KIO" or "KPO".
  - **Sequence Size**: The length of the number, i.e., how many digits must be printed after the prefix.
  - **Step**: The frequency at which the numbers change, usually set to 1.
  - **Next Number**: The next number in the sequence, based on the company’s existing numbering system. If there is no previous sequence, enter 1.
  
  For example, in the image, the next document will be numbered KIO0054.

Main Functions
--------------

- When creating a new payment in the Cash Journal, depending on the payment type - send or receive - a KIO or KPO number is automatically assigned when the payment record is confirmed.

- When creating a payment where the type is set to "send" and the journal is Cash, upon confirmation, a KIO number is automatically assigned according to the defined sequence.

  .. image:: l10n_lt_kio_kpo_receipt/image03.jpg

- You can print such a document by clicking the **PRINT** button in the record and selecting the KIO/KPO print format.

  .. image:: l10n_lt_kio_kpo_receipt/image04.jpg

- When creating a payment where the type is set to "receive" and the journal is Cash, upon confirmation, a KPO number is automatically assigned according to the defined sequence.

  .. image:: l10n_lt_kio_kpo_receipt/image05.jpg

- You can print such a document by clicking the **PRINT** button and selecting the KIO/KPO print format.

  .. image:: l10n_lt_kio_kpo_receipt/image06.jpg


Daily Use Scenarios
-------------------

- After a payment is confirmed and a KIO or KPO number is assigned, it is no longer possible to change the payment type (even if the payment is restored as a draft) because the assigned KIO or KPO number does not update. If a mistake was made, the KIO or KPO number will be used and cannot be reused in the future. In such a case, the payment should be canceled, and a new, correct payment should be created.

Integrations and Connections with Other Modules
-----------------------------------------------

- The module is linked to the Cash Report (see more in the Cash Book documentation).

Updates and Version Control
----------------------------

- The module is updated with each new version of Odoo.
