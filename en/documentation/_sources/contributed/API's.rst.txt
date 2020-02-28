API's
=====
=============
Create Entity
=============

::

	POST  /domain/entity


Parameters
----------


.. csv-table::
   :header: "Name", "``*``", "Type", "Description"
   :widths: 25, 3, 25, 75
   
   "identity", "``*``", "string", "value identifying entity at creation time"
   "requestor", "``*``", "string", "idempotent identity of the requestor creating the entity"
   "passCode", "``*``", "string", "not sure what this is"

	 
Response
--------

.. code-block:: json

   {
      "EDIDcreated": "PKyPcRCSgPeYlBMe8wetgPaaFBQffxQXcPWsePcODwWZW",
      "rpCode": "FWDXytCcR48"
   }


	 
.. keep the following at the bottom of the page

[*] indicates a mandatory versus optional parameter