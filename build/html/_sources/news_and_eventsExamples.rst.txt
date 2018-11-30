News & Events Examples
======================

Create RSS or iCal Feed
-----------------------
#. Navigate to the News Feed/Events Feed tab

    * Located in **Settings**

#. Click the **+ Feed** button in the bottom right corner
#. Type in a title representative of the feed
#. Paste in the URL of the

    * iCalendar Feed
    * RSS Feed
    * The button at the right will open or download the URL link

#. Choose the refresh frequency

    * Daily
    * Hourly

#. Add a `Remove Text` sequence if necessary

    * Optional

#. Add any additional categories to be associated with this feed

    * Optional
    * Events Categories can be added in **Slots** > **EVENT_CATEGORY** Predefined Slot found towards the bottom
    * News Categories can be added in **Slots** > **NEWS_CATEGORY** Predefined Slot

#. Add a template that will be applied for all feed items
    
    * Optional

    Template Example::

        ## iCal has fields time, location, description, title
        ## RSS example works similarly
        ## This is just an example, fields may be named differently
        Location: {{location}}
        {{description}} The event will take place at {{time}}.

    Each event will now look like the following example:

    **Location: PACE Center**
    **Get into the holiday spirit as the Chorale and the Symphony treat you to an evening of traditional carols, songs, and a few surprises. The event will take place at 7:30-9:30.**

#. Click Save
#. The new feed will now be in the feed grid
#. Sync feed to see events in events grid, or news in news grid

    * Click sync button in row of feed
    * Toast Message will appear when feed has been synced

#. Verify that feed has been synced by navigating to **Events**/**News** in left menu
#. Clear feed by clicking the 'no symbol', which is a circle with a slash

.. image:: ./images/ical_feed.gif


Create News Records
-------------------

#. Navigate to **News** in the left menu
#. Click **+ News** in the bottom right
#. Fill out fields
    
    * Title
    * Link - is applicable
    * Publish Date - the date that will be relevant
    * Voice and Display Message
    * News Category - will help narrow a user's news question; can be set in Slots as **NEWS_CATEGORY**

#. Save

**Note**: Only custom news can be edited at the current time. Feed news are not editable.

.. image:: ./images/create_news.gif

Create Events Records
---------------------

#. Navigate to **Events** in left menu
#. Click **+ Event** in the bottom right
#. Fill out fields

    * Title
    * Category - can be set in slots as **EVENT_CATEGORY**
    * Area - city, general locations, can be set in Slots as **CITY**
    * Location - address or specific location
    * Voice and Display Message
    * Start Date
    * End Date
    * Approved - approval will allow it to be a searchable event

#. Save

    **Note**: Only custom events can be edited at the current time. Feed events are not editable.   

.. image:: ./images/create_event.gif