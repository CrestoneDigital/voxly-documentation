Events Examples
===============

Create iCal Feed
----------------
#. Navigate to the Events Feed tab

    * Located in **Settings**

#. Click the **+ Calendar Feed** button in the bottom right corner
#. Type in a title representative of the feed
#. Paste in the URL of the iCalendar Feed

    * The button at the right will open or download the URL link

#. Choose the refresh frequency

    * Daily
    * Hourly

#. Add a `Remove Text` sequence if necessary

    * Optional

#. Add any additional categories to be associated with this feed

    * Optional
    * Events Categories can be added in **Slots** > **EVENT_CATEGORY** Predefined Slot found towards the bottom

#. Add a template that will be applied for all feed items
    
    * Optional

    Template Example::

        ## iCal has fields time, location, description, title
        ## This is just an example, fields may be named differently
        Location: {{location}}
        {{description}} The event will take place at {{time}}.

    Each event will now look like the following example:

    **Location: PACE Center**
    **Get into the holiday spirit as the Chorale and the Symphony treat you to an evening of traditional carols, songs, and a few surprises. The event will take place at 7:30-9:30.**

#. Click Save
#. The new feed will now be in the Calendar Feed grid
#. Sync feed to see events in events grid

    * Click sync button in row of feed
    * Toast Message will appear when feed has been synced

#. Verify that events have synced by navigating to **Events** in left menu
#. Clear feed by clicking the 'no symbol', which is a circle with a slash