This is an adaptation of InaneCoding Piwik Opencart module to make it compatible with OC 2.x
Should be compatible with OC 2 up to 2.0.1.1 version (included).
Not tested on OC 2.0.2.x (which is still unstable) 


Author: OpenSource Experts (http://www.expertsos.net)
Version: 0.1
Based on: InaneCoding Piwik OpenCart module version 1.1
Release Date: 2015-04-28
License:			GNU General Public License (GPL) version 3


From orginal InaneCoding readme:

------------------------------------------------------
InaneCoding Piwik OpenCart Ecommerce VQmod
------------------------------------------------------
Source Repository:	https://github.com/InaneCoding/Piwik-OpenCart-Ecommerce-VQMod
Author:				Kevin Bibby / InaneCoding.co.uk
Version:			1.1
Release Date:		2014-06-25
License:			GNU General Public License (GPL) version 3
------------------------------------------------------

DESCRIPTION
-----------
Implements Piwik Ecommerce tracking for OpenCart;
> Tracks regular page views
> Tracks Ecommerce product views (category views not yet implemented)
> Tracks Ecommerce cart add/update/delete
> Tracks Ecommerce orders
> Tracks Site Searches
OpenCart admin backend for modifying settings.
Option to use Piwik Proxy Hide Url script to obfuscate the URL in the javascript code.
Fully VQmod'ed up! Does NOT overwrite any core files.



IMPORTANT
---------
1. Requires VQmod installed (Highly recommended - https://code.google.com/p/vqmod/ ).

2. Requires Piwik installed.

3. The default install assumes that Piwik is installed to the '/piwik/' folder at the root of your OpenCart site.
If you have used a custom install path then please place the 'PiwikTracker.php' file from '/upload/piwik/PiwikTracker.php' to your custom Piwik folder.

4. The default install assumes that your OpenCart Admin directory is in the '/admin/' folder at the root of your OpenCart site.
If you have used a custom Admin path then please place all files from '/upload/admin/' to your custom OpenCart Admin folder.

INSTALL
-------
1) Upload the contents of the 'Upload' directory to the root of your OpenCart site.
2) Go to the Extensions -> Modules page, and click 'Install' next to 'Piwik OpenCart Ecommerce mod'.
3) After install, click 'Edit' next to 'Piwik', and on the settings page enter the details about your site and the Piwik installation;

a) "Piwik installation URL" - This is the full url to your Piwik installation (without 'http://'). e.g. "www.example.com/piwik/".
b) "Full path to the PiwikTracker.php file" - As the name says, this is your server filepath to your PiwikTracker.php file in your Piwik folder - commonly this will be "/home/~user/public_html/piwik/PiwikTracker.php", where '~user' is replaced by your website hosting username. However this can vary depending on the server configuration.
c) "Piwik auth token" - This is your secret Piwik authorisation token. Get this from the 'API' tab on your Piwik admin panel.
d) "Piwik Site ID" - This is the ID used in your Piwik install for the site you want to track, usually this is '1' but can vary if you have multiple sites or a custom setup. Consult the 'Website Management' page on your Piwik admin panel for this setting (under Settings -> Websites).
e) "Piwik Tracking" - Global 'Enabled' / 'Disabled' setting for the Piwik OpenCart mod.
f) "Ecommerce tracking" - Set this to 'Enabled' to allow tracking of Ecommerce actions such as product views, cart operations and orders. Set this to 'Disabled' if you only wish to track regular page views.
g) "Piwik Proxy Script" - Set this to 'Enabled' to route all Piwik tracking requests through the Piwik Proxy script at the root of your site; useful if the "Piwik Installation URL" is at another URL/server which you don't want to make public.
h) "Piwik SKU" - Select what product field you would like to use when reporting the SKU (Stock Keeping Unit) in an Ecommerce operation. This can use either the 'Model' or 'SKU' fields which every product in OpenCart has.



UPGRADE
-------
To upgrade from a previous version simply upload the files from the new version as described in step 1) of the installation.
There should be no need to re-install anything else or change/restore any settings as I've tried to pay attention to backwards compatibility during development.
Please get in touch if you experience any issues.



UNINSTALL
---------
In OpenCart admin, go to the Extensions -> Modules page, and simply click 'Uninstall' next to 'Piwik OpenCart Ecommerce mod'.
This will ensure the configuration settings are deleted and that none of the main functions of the mod will run.
Some files will still remain - however these should be perfectly safe and not affect anything but to fully remove please delete all files which you uploaded during the install.



LIMITATIONS
-----------
This is one of the first widespread release but would still benefit from further feedback. Please report any bugs found!
1) There is no functionality (yet) to track the category during page views / cart updates / orders.
2) Some small limitations to site search;


WITH THANKS TO
--------------
Gordon Downie - for his brilliant code contribution to add the install and settings functionality to OpenCart admin.
Github User glennw - for his bug report and fix for 'mod disabled' footer comment.

