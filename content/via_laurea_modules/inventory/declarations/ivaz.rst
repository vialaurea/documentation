i.VAZ
=====

Introduction
------------

i.VAZ can be filled in both Accounting and Inventory modules. It is most convenient to fill i.VAZ in the Inventory module..

An important condition is that i.VAZ can only be filled after confirming the delivery document or OUT in the Inventory module. The delivery order OUT must be in "Done" status.

  .. image:: ivaz/image03.jpg

Daily Use Scenarios
-------------------

After preparing the sales order and confirming the goods shipments in the Sales module, you can see them in the Inventory module, Operations section, under Deliveries.

  .. image:: ivaz/image15.png

When you select this section, you will see a list of deliveries. From the list, select and mark the deliveries for which you want to create an i.VAZ file. Then click the "Generate i.VAZ" button.

    .. image:: ivaz/image16.jpg
  
Choose whether you want to generate a batch or separate i.VAZ documents.

    .. image:: ivaz/image17.jpg
  
1. If you choose to generate an i.VAZ batch, a common draft i.VAZ record will be automatically created for all marked deliveries. Fill in the required fields in it. If needed, adjust the shipping and delivery dates and times.

In the Transfers tab, you will see the list of deliveries you have selected.

    .. image:: ivaz/image18.jpg
  
Go to the "Waybills" tab, click the "Generate Documents" button, and the delivery list will be transferred to waybills.

    .. image:: ivaz/image19.jpg

After doing this, confirm the document and a "Download Document" button will appear at the top of the window. Clicking it will download the i.VAZ file to your computer, which you can then upload to the VMI system.

  .. image:: ivaz/image20.jpg

2. If you choose to generate separate i.VAZ documents at the time of creation, you will need to enter delivery data separately for each delivery. We recommend using this option when shipments will be delivered by different carriers or vehicles.

In this case, i.VAZ drafts will be created for each delivery.

  .. image:: ivaz/image21.jpg

In each delivery, check the "Strict Verification" option and fill in the required fields.

  .. image:: ivaz/image22.jpg

The shipping and delivery address information is automatically read based on your company's warehouse and recipient's contact card details and addresses. If needed, adjust the shipping and expected delivery dates and times.

After filling in the data, click the "Confirm" button. An additional "Download Document" button will appear at the top of the window, which will allow you to download the document to your computer and upload it to the VMI system.

  .. image:: ivaz/image23.jpg

Other, additional filling options
-------------------

Additional filling options can be found at:

1. Accounting module menu i.MAS >> i.VAZ

  .. image:: ivaz/image01.jpg

2. In the inventory module, by selecting the i.VAZ menu.

  .. image:: ivaz/image02.jpg

In both cases, i.VAZ is formed by selecting the appropriate option - as a batch or as a document, based on the needs described above.

If filling as a batch, in the i.VAZ section select i.VAZ batch documents and click the "New" button.

  .. image:: ivaz/image04.jpg

In the opened window, enter the carrier, vehicle license plate number, make, and driver's first and last name. Click "Add or Remove Documents".

  .. image:: ivaz/image05.jpg

A new window will open where you should click the "Add a line" link.

  .. image:: ivaz/image06.jpg

A new window will open where you can create a new waybill. In the transfer, select the confirmed sales order waybill number, fill in the recipient, sender, transportation dates and times, and check the shipping and receiving locations in the detailed information at the bottom (they are automatically taken from the customer card). If necessary, adjust the addresses.

  .. image:: ivaz/image07.jpg

After filling in, save the document. You will see the entered document in the list of added waybills. If needed, you can add more waybill lines. After uploading all required waybills from sales orders, confirm the document.

In the i.VAZ documents window, you will see all uploaded waybills in the waybill lines. After checking, confirm the document.

  .. image:: ivaz/image08.jpg

After confirmation, a "Download" field will appear. Clicking it will download a file in xml format to your computer, which you can upload to the VMI system.

  .. image:: ivaz/image09.jpg

After sending, click the "Document Sent" button. In the i.VAZ section, by selecting "i.VAZ documents" you can check the sending information of a specific waybill:

  .. image:: ivaz/image10.jpg

And, if needed, download the file again in xml format for submission:

  .. image:: ivaz/image11.jpg

If you are transferring your goods from one location to another, select the "Transfers" tab and click "Add a line".

  .. image:: ivaz/image12.jpg

Mark the appropriate Transfer waybills and click "Select" or create a new one where you will enter the data manually.

  .. image:: ivaz/image13.jpg

You will see the added waybills in the list:

  .. image:: ivaz/image14.jpg

Fill in all i.VAZ fields according to the description provided above. Confirm, generate the xml file and attach it in the VMI system.

Automatic submission option
-------------------

There is a possibility to perform additional configurations that would allow uploading the i.VAZ file directly to the VMI system from Odoo with a single button click. If needed, contact Via laurea for additional configurations.
