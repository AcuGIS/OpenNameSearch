OpenNameSearch
===========================
This script is for building a basic Nominatim server with OpenStreetMap data.

Only for use on a clean Ubuntu 14!

Before proceeding, see http://opennamesearch.org for limitations, etc..

An Ubuntu 16 version has been contributed by @f1ana: https://github.com/f1ana

https://github.com/AcuGIS/OpenNameSearch/blob/master/OpenNameSearch-Ubuntu16.sh


Installation
------------


Step 1: Get the OpenNameSearch.sh script from GitHub::

	https://github.com/AcuGIS/OpenNameSearch/blob/master/OpenNameSearch-Ubuntu16.sh

Step 2: Make it executable::

	chmod 755 OpenNameSearch.sh

Step 3: Run the script::

	./OpenNameSearch pbf_url

Examples
------------

Load Delware data::

	./OpenNameSearch.sh http://download.geofabrik.de/north-america/us/delaware-latest.osm.pbf

Welcome Page
------------

Once installation completes, navigate to the IP/nominatim or hostname/nominatim on your server.

You should see a page as below:

.. image:: http://opennamesearch.org/assets/img/Nominatim-Welcome.jpg


Loading and Reloading PBFs
--------------------------

You can use our reload-OpenNameSearch.sh script via GitHUB script.

Usage is::

	./reload-OpenNameSearch.sh [PBF_URL1] [PBF_URL2] ...


Enable Automatic Updates
------------------------

The script creates an updater service.  In order to enable updates::

	chmod +x /etc/init.d/nominatim_updater


Credits
-------

https://www.acugis.com

https://citedcorp.com


Contribute
----------

- Issue Tracker: github.com/AcuGIS/OpenNameSearch/issues
- Source Code: github.com/AcuGIS/OpenNameSearch

Support
-------

If you are having issues, please let us know.

License
-------

The project is licensed under the BSD license.
