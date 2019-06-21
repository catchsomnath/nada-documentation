Requirements
###############

NADA requires PHP, a MySQL database and a web server. 


PHP requirements
--------------------

The minimum required version is PHP 7 with the following PHP extensions enabled:

* xsl
* xml
* mbstring
* mysql 

For Microsoft SQL Server, you'll need **sqlsrv** extension for PHP.

.. note:: 

	See section on PHP configurations for configuring your server for NADA.


Web Server requirements
--------------------------
* Apache 2.4 or later
* IIS 6/7.x or later
* NGINX 



Supported Databases
---------------------
* MySQL 5.x
* Microsoft SQL Server with fulltext support

For MySQL, NADA supports version below 5.6 (no longer supported by MySQL community) but for better performance use the latest 5.7 or MySQL 8.
