Data Deposit Installation
##############################

NADA includes the data deposit as of V5.0.4. The data deposit is not installed by default and must be installed and enabled manually.


Install data deposit database
==============================

* Run the SQL from the file `install/schema.dd.mysql.sql` on your NADA database. This will create all the tables used by the data deposit.


Enable data deposit
===================

* To enable data deposit, edit the configuration file `application/config/datadeposit.php`.

* Change the setting **enable_datadeposit** to **TRUE**:

::

	$config['datadeposit']['enable_datadeposit'] = TRUE;


* Save the file.

* Open web browser and navigate to **your-nada-web-folder/datadeposit** to see data deposit frontend.



