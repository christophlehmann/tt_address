.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

.. include:: ../../Includes.txt


.. _configuration-extension-configuration:

Global extension configuration
==============================

After the installation has been completed, some global configuration can be defined.

If you are using TYPO3 8.7, this configuration can be found in the Extension Manager.
With version 9.5 this has been moved to the Install Tool.

Settings
--------

The following settings are available:

======================================  ==========  =============================================================  =========================
Property:                               Data type:  Description:                                                   Default:
======================================  ==========  =============================================================  =========================
activatePiBase                          boolean     If set, the ancient plugin based on `AbstractPlugin`,          0
                                                    formerly known as `piBase` is enabled and can be used.
                                                    However, be aware that this plugin has been marked as
                                                    deprecated and will be removed in version 5.0.0.
                                                    Try not using this plugin!
--------------------------------------  ----------  -------------------------------------------------------------  -------------------------
storeBackwardsCompatName                boolean     If set, the field `name` is populated with the values of the   1
                                                    fields `first_name`, `middle_name` and `last_name`.
--------------------------------------  ----------  -------------------------------------------------------------  -------------------------
backwardsCompatFormat                   string      Define the format how the name field is populated.             %1$s %3$s
                                                    Use `%1$s` for the first name, `%2$s` for the middle name
                                                    and `%3$s` for the last name.
--------------------------------------  ----------  -------------------------------------------------------------  -------------------------
readOnlyNameField                       boolean     If set, the name field is set to read only which makes         1
                                                    absolutely sense if the value of the field is populated
                                                    automatically.
======================================  ==========  =============================================================  =========================
