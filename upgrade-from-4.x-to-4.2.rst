==============================
Upgrade from NADA 4.x to 4.2
==============================


The patch includes a subset of files changed from version 4.x to 4.2. Download the patch - Download the patch http://www.ihsn.org/download/nada42.1-patch-APR-24-2014.zip


To apply the patch, follow the steps:

1. Make a backup of your existing NADA folders. If complete backup is not possible, at least back the "Application" and "Themes" folder

2. Unzip the files in the NADA root folder to replace existing files

3. Set write permissions on the language folder located at /application/language. This is needed for the upgrade script to update language files with new translations.

4. Run the upgrade script from http://[nada-url]/index.php/nada42_upgrade/run


.. note::

    The patch does not overwrite the settings for database, config and template configurations.


**4.2 Change log**

The update includes the following fixes:

* Email settings can be setup using a config file instead of using the site configurations

* User passwords are hashed using a stronger encryption

* Updated Licensed Data Access administration page to filter requests by status type and increase number of requests listed on the page

* Added support for bulk requesting licensed datasets

* Added page for creating bulk data access collection on the site administration under studies menu

* Misc. formatting enhancements for the licensed access request forms and email messages

* Replaced CI SMTP library with PHPMAILER

* Misc. bug fixes for Manage study page

* Fixed double download counts for data file downloads

* Moved DDI|RDF under the tab "export metadata" on the study information page

* Excluded PDF documentation, DDI and RDF downloads from study download counts to make the download counts consistent with the study download reports

* Updated tab labels on study infor page for data dictionary and study description and re-arranged tabs to make the external resources the default tab

* Fixed: Sorting is not remembered on browser back button for data catalog search page

* Fixed: On data catalog page, sometimes country selection dialog box shows up empty/blank

* Fixed: Refresh DDI changes the study ownership to 'default'

* Fixed: Batch refresh ddi assigns the study to 'DEFAULT'

* Updated variable information display: re-arranged elements to move categories list under literal question

* Fixed: Country mappings page does not work on IE [/admin/countries/mappings]

* Added a link to fix country mappings page [/admin/countries/mappings] on countries index page

* Updated: Replace DDI would not allow replacing a DDI with the same ID.

* Fixed: On Manage Study page, data access types filter resets on page navigation

* Fixed: On Manage Study page, page size resets on searching

* Fixed: On Manage study page, dilters reset to none if user navigate to see more results

* Fixed: Tags are not deleted on deleting a study

* Added field/element "translated title" on study overview tab

* Added field/element "Questionnaires" on study data collection tab

* Added field/element "Version notes" on study overview tab

* Renamed section "Access policy" to "Data Access" and updated formatting for the data access page

* Updated: All fields from the Nesstar "IHSN 1.6 EN" template are displayed in NADA

* Added: No captcha option to show no captcha on register page if image or google recaptcha are not available

* Fixed: On copy studies to collection page - search does not work

* Fixed: Dashboard shows wrong number of studies with no questionnaires

* Fixed: Batch import DDI does not import all RDF entries

* Fixed: Duplicate external resources are not imported

* Fixed: Reset button missing from the variable search on study description page

* Fixed: PDF generator shows a blank page and does not generate a PDF

* Removed carousel from the home page by default and can be enabled by editing the home page file.