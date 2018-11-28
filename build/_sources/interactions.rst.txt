Interactions
============

This section was designed to best assist how to create and edit interactions. Using slot values created within the Slots section in Settings, the ability to identify the information community members will be requesting will be made easy to create responses for. Voxly will give the ability to type the response to the interaction and connect any open source data to communicate. 


Every skill starts with two interactions: Help and Welcome. Specify the skill help and welcome messages.

.. image:: ./images/interactions.png

================================
Features Within Interaction Grid
================================

* Filter Interactions
    * Interaction Status
        * Click on buttons to the top left
            * All | Pending | Approved

    * Intents Filter
        * Click in the intent combo-box and down arrow-key to the intent and hit `enter`
        * Type name of intent and hit `enter`

    * Search Bar
        * Search word in display and voice message

        .. image:: ./images/interaction_grid.png

===================
Interaction Caching
===================

What is interaction caching? Interaction caching is the process of saving the response to an interaction. This saved response is then used the next time that same question is asked. By saving certain responses we improve performance (response time) and resource consumption (reduced database access and server load). Response times are improved because we already have the answer before the interaction is asked. Resource consumption is reduced because we do not need to query the database for our response and the server is freed up to handle other requests improving response times. Responses that are saved have a time to live (ttl). The time to live (ttl) is used to determine how long a saved response should be used. The saved response is deleted after the time to live (ttl) expires. When any interactions are edited in the manager and saved, any cached results related to that interaction are also cleared out in order to show the latest information. This is also true for when News Feeds or Event Feeds are updated.

When to use caching? Interaction caching should be used when a response to an interaction is independent of the user asking the question. If two people asked the same question would they get the same response? If the answer is yes then that interaction can probably be cached. An example of a cache-able interaction is ‘Tell me today’s news’. If five people asked this question, they would all get the same response. If the question was changed to ‘Tell me news near me’ then the response would not be cached because it refers to specific user information.    

How long should a response be cached (time to live or ttl)? The time to live is determined by how long that response is valid. It is recommended to make the time to live shorter rather then longer. Better to send a fresh response to the user rather than one that's out of date and stale. If the interaction uses a connector and the data is updated every hour then setting the cache to be between 5 min to 1 hour is recommended depending on how frequently it should use the latest data. If the data updates every day then typically the ttl should be set to a more frequent time.

In an effort to track and improve caching, Voxly tracks when a cached response or a fresh response is sent to the the user and is shown in the logs.

View the Interaction Guides here:    :ref:`Interaction Guides`