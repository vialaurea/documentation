i.VAZ
=====

Introduction
------------

- i.VAZ can be filled in the Accounting and Inventory modules.
- You can find the filling option in the Accounting module under the i.MAS section.
  .. image:: ivaz/Image01.jpg
- Or in the Inventory module under the i.VAZ section.
  .. image:: ivaz/Image02.jpg

Daily Use Scenarios
-------------------

- In both modules, the file is generated differently. An important condition is that i.VAZ can only be filled after confirming a sales order in the Sales module. The sales order must be marked "Done":
  .. image:: ivaz/Image03.jpg

- i.VAZ is generated identically in both the Inventory and Accounting modules:
  - In the i.VAZ section, select "i.VAZ batch documents" and click the "New" button.
    .. image:: ivaz/Image04.jpg
  - In the window that opens, enter the carrier, vehicle registration number, make, driver's name, and surname. Click "Add or remove documents".
    .. image:: ivaz/Image05.jpg
  - In the next window, click the "Add line" link.
    .. image:: ivaz/Image06.jpg
  - In the next window, you can create a new waybill. In the transfer, select the confirmed sales order waybill number, fill in the recipient, sender, transportation dates and times, and check the detailed information for dispatch and receipt locations at the bottom (these are automatically taken from the client's card). Correct addresses if necessary.
    .. image:: ivaz/Image07.jpg

- After filling in, save the document. You will see the entered document in the list of added waybills. If necessary, you can add more waybill lines. After loading all the required waybills from the sales orders, confirm the document.
- In the i.VAZ document window, you will see all the uploaded waybills in the waybill lines. After checking, confirm the document.
  .. image:: ivaz/Image08.jpg

- Once confirmed, a "Download" field will appear. Click on the link to download an xml file to your computer, which you can upload to the VMI system.
  .. image:: ivaz/Image09.jpg

- After sending, click the "Document sent" button. In the i.VAZ section, select "i.VAZ documents" to check the dispatch information of a specific waybill:
  .. image:: ivaz/Image10.jpg

- And, if necessary, download the file for submission in xml format again:
  .. image:: ivaz/Image11.jpg

- If you are transferring your goods from one place to another, select the "Transfers" tab, click "Add line".
  .. image:: ivaz/Image12.jpg
- Check the appropriate Transfer waybills and click "Select" or create a new one where you manually enter the data.
  .. image:: ivaz/Image13.jpg

- You will see the added waybills in the list:
  .. image:: ivaz/Image14.jpg

- Fill in all the i.VAZ fields according to the above description. Similarly, confirm, generate the xml file, and attach it in the VMI system.