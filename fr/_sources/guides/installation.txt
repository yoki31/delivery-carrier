.. _installation:

############
Installation
############

In order to install PostLogistics WSBC module, make sure you have the following requirements and Odoo dependencies on your system.

************
Requirements
************

To use this module you need to install `suds-jurko`_ library
(A library to manage SOAP calls)

Make sure you use it over the unmaintained `suds` library.

.. _suds_patch:

.. important:: In case you want to use the test mode for developpement purpose, you will have to patch the library with the following patch.

    https://fedorahosted.org/suds/attachment/ticket/239/suds_recursion.patch


*****************
Odoo dependencies
*****************

This module depends on module `base_delivery_carrier_label` you will find in the same module repository on https://github.com/OCA/carrier-delivery/

Plus, if you are not using this module with automated tools, you will want to install **Attachments List and Document Indexation** (`document`) module. Otherwise you want be able to use the labels as they are created as attachments.

Next step
=========

:ref:`configuration`

.. _`suds-jurko`: https://pypi.python.org/pypi/suds-jurko
