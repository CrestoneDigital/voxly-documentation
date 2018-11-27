Interaction Examples
====================

Name the connectors to be unique and specific to what they are used for. Multiple connectors may be created of the same type.

===============
Carto Connector
===============

.. image:: ./images/census_carto_1.png


.. image:: ./images/census_carto_response_2.png

========
Airtable
========

.. image:: ./images/integration_airtable.gif

The API Key is located in the Airtable User Account. Click on the User Image in the top right, and click on **Account**. API Key is located in the Overview section under API. For first time, click **Generate API key** or use the personal API key that's been generated. The API Key and Airtable API link to get the Base ID is highlighted in the image below. 

.. image:: ./images/airtable_api_key.png

To get the Base ID, press the `Airtable API` above where the API Key is in the User Account Settings. Once pressed, a new tab will open. The Airtable API for "TABLE NAME" will be displayed at the top. To change which table or data-set, press the down arrow. Scroll down on the right side, the Base ID is highlighted in the Example Using Bearer Token Example.

.. image:: ./images/base_id_airtable.png

Once the Airtable Connector has been created, navigate to interactions to begin creating new interactions using the new connector.

.. image:: ./images/airtable_1.gif

* Drag and Drop the Airtable connector into the flow diagram area
* Connect the Start component to Airtable, and Airtable to Response
* Table is the name of the table tab in the airtable table
* Fields are the columns. To add fields, type the name of the column and hit the **Comma Key** on the keyboard. This will create a boxed item with the name and an 'x' to be able to remove it from the list. Add as many fields as may be useful for this interaction response.
    * Add `Category`
    * Add `brand_description`

* View should be the `Grid view.`
* Filter on a particular value. Ex.) Category = "BRANDY" should return all records with category matching "BRANDY" and the records brand_description

=============
ArcGIS Online
=============

====
CKAN
====

=======================
Google Sheets Connector
=======================
The spreadsheet ID is highlighted in the Google Sheet URL. The value is followed by the spreadsheets/d/{spreadsheet ID}/

.. image:: ./images/google_sheet_id.png

The Google Sheet GID, which is used within the interaction is the right number highlighted in the image above. It can be found by copying the number after the **#gid={gid}**.

The GID will change when changing table tabs which are located at the bottom left.



======
Lambda
======

============
OpenDataSoft
============

========
PostGres
========

========
REST API
========

==========
Salesforce
==========

=================
Socrata Connector
=================
