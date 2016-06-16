.. _configuration:


#############
Configuration
#############

Here you will find how to configure PostLogistics WSBC module we just have installed.

The configuration is done in:

* for Odoo 7.0 and 8.0 in *Settings/Configuration/Carriers/Postlogistics*
* for Odoo 9.0 in *Inventory/Settings/Carriers/Postlogistics*

.. image:: ../_static/img/postlogistics_settings.png
   :alt: *Inventory/Settings/Carriers/Postlogistics*

**************************
Web Service Authentication
**************************

Fill user and password with the credentials provided by PostLogistics.

If you want to use a test account you have to activate the "Test Mode" check box.

.. warning:: If you want to use test mode, your setup needs a patch on library ``suds-jurko``.

    See `suds patch <installation.html#suds_patch>`__.


******************
Frankling Licenses
******************

Add one or multiple Franking license. A license is a number of 8 digits provided by PostLogistics.
For each license PostLogistics can enable the use of some basic services.
You can have multiple license. Those will be selectable on setup of delivery methods, so name them properly.

.. image::  ../_static/img/postlogistics_licenses.png
   :alt: PostLogistics frankling licenses

******************
Sender Information
******************

In Sender information you can optionally define the logo of your company displayed on labels.

.. warning:: Be advised that the format is very restrictive, here are the rules:

    If using an image / logo, please note the following:

    * Image width: 47 mm
    * Image height: 25 mm
    * File size: max. 30 kb
    * File format: GIF or PNG
    * Colour table: indexed colours, max. 200 colours
    * The logo will be printed rotated counter-clockwise by 90°

PostLogistics recommendations are of using a black and white logo for printing in the ZPL2 format.

If the logo is not set, company address will be printed on the label.

Plus you need to specify the Domicile Post office, ask PostLogistics if you are not sure.  E.g. 3030 Bern

***************
Default configs
***************

Default configurations contains format options of labels output.
Those will be applied on all labels defined in all your delivery methods unless you override it by specifying
those format options in delivery method or on the picking.

****************
Tracking numbers
****************

The option tracking numbers allows you choose how is generated the last 8 digits of the tracking number.

You have two options.

The first is by default, you let PostLogistics define random numbers.
The second is to tell Odoo to generate it and send it to the WSBC in the following format.
The 2 first digits are for a pack counter the last 6 digits are for picking number.

E.g. ``07000042`` would be the 7th pack of the picking OUT/042

.. note:: You can create your own module to change the generation of tracking numbers by redefining ``_get_number_item()`` method.

**********************************
Synchronize Odoo options with WSBC
**********************************

Once your credentials are set, this will get you the all the WSBC options data at once. You must do this action before you configure the delivery methods.

.. image:: ../_static/img/postlogistics_settings_update_service.png
   :alt: Button Update PostLogistics Services


*********************************
Assign licenses to Service groups
*********************************

If you have multiple licenses and those licenses match with a type of service, you might want to auto configure this.
Thus you won't have to select the license when configuring your delivery methods.

.. image:: ../_static/img/postlogistics_settings_assign_licenses.png
   :alt: Button Update PostLogistics Services


Next step
=========

Can we print label now?

No, we are not done yet. The next step is :ref:`delivery_method_setup`.
