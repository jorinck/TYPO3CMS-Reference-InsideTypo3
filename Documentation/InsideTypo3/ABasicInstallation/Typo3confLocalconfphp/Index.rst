.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

.. include:: ../../../Includes.txt
.. include:: Images.txt


typo3conf/localconf.php
^^^^^^^^^^^^^^^^^^^^^^^

Lets create a localconf.php file::

   <?php

       // Setting the Install Tool password to the default "joh316"
   $TYPO3_CONF_VARS['BE']['installToolPassword'] = 'bacb98acf97e0b6112b1d1b650b84971';

       // Setting the list of extensions to BLANK (by default there is a long list set)
   $TYPO3_CONF_VARS['EXT']['extList'] = 'install';
   $TYPO3_CONF_VARS['EXT']['requiredExt'] = 'lang';

       // Setting up the database username, password and host
   $typo_db_username = 'root';
   $typo_db_password = 'nuwr875';
   $typo_db_host = 'localhost';
   ?>

Without the correct MySQL username and password we would get this error:

|img-5a|

The result will be this:

|img-5b|

So we are connected to the server (username and password accepted) but
we have not yet defined a database. Lets go create a blank one!

