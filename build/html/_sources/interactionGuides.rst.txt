Interaction Guides
==================

=============================
Create Interaction and Answer
=============================

#. Choose interaction type
    * Located in the bottom right, press and choose the interaction type

#. Fill out interaction template
    * Located at top
    * Select office the interaction is addressing
    * Slot Types that are predefined will be look like *{Date}*
    * Select Slot Values from the drop-down   
        
        *Multiple verbs can be chosen, if fitting to question being established*
    * Click box to make the answer to the FAQ available to your Alexa skill. 
    * If box is left unchecked the created response will be saved and can be edited.
    
    *Interaction will not be acknowledge by your skill until approved*
    
    * You can specify if the interaction should be cached and for how long

    *Slots filled within the template give Alexa context to search for information*

#. Fill out Flow - Interaction Flows
    #. Components - Located in left menu under **Components**
        To fill out components in the flow, mouse over. The left button, pencil icon, if to edit; the right button, x icon, is to delete the component. To connect components click the initial component anchor and click again on the next component. To remove a connecting line,  right-click the starting anchor and press delete.

        .. image:: ./images/delete_component.png

        * Response
            * Voice Message - Spoken message for a response
            * Card Title - Header for the message on devices with a screen
            * Display Message - Message to be shown on devices with a screen
            * Image URL - Image shown on devices with a screen, the sizes are for varying device screen sizes
                * Small Image - recommended size: 720 width x 480 height
                * Large Image - recommended size: 1200 width x 800 height
            * Accessibility Text - Description of the image (For Screen Readers)
            * Display Templates - Defaults to a Card Template

            If display card template is selected, it will enable/disable certain fields.
                * Background Image URL - The image that will be used as the background. The right button will open the link in a new tab to display image
                * Accessibility Text - The description of the image (For Screen Readers)

            * Directives - Playing video, audio, or third party services such as spotify
                * URL - the link
                * Title - header to be shown on devices with a screen
                * Subtitle - 
            
        * Link Account - Third Party Account Linking
            * Voice Message - Prompt message for third party account Linking

        * Loop
            * List - Collection or list of Items; ex. News or Events have multiple items to iterate through
                * Path - Specifies how to interpret the text; considered input. Ex.) connectors.data is the list
                * Function - Interpret input as a function to be called, some functions may take arguments. **See Data**
                * String - Interpret input as String
                * Number - Interpret input as a Number

            * Prompt for Next - Response for next item if there is more items. Ex.) "Would you like to hear the next item?"
            * Card Title
            * Voice Message
            * Display Message
            * Image URL
            * Directives
                * Play Spotify
                    * Playlist - URL
                
                * Play Video
                    * URL
                    * Title
                    * Subtitle
                
                * Play Audio
                    * URL
                    * Title
                    * Subtitle
                    * Image URL
                    * Background Image URL
                    * Pause Response - Response for when directive is paused
                    * Resume Response - Response for when directive is resumed
                    * TTL After Pause - Time to Live; how long before the directive is cleared and can't be resumed
                
        * Yes/No
            * Yes
            * No 
            * ??? - Other response

        * Check Intent
            * Intent Dropdown - Allows manager to make path decisions for an interaction. Can add several different intents and have a response if the user spoke one of the specified intents, or not.

        * Add Variables - Create inputs to be used in functions and responses
        * Save Settings - Similar to `Add Variables`
            * Setting Values - create visitor_settings for users for later use. There is a name, the input, and the input type.

        * Connectors
            * c1 - The name of the connector to be used in {{connectors.c1}}
            * Connector Info - fill out the requirements for the connector
    
    #. Data - Located in the left menu as the right tab under **Data**, right of **Components**. Items are drag-n-droppable for components, these can be use to create queries, and add to the responses of the interactions. 
        
        * Inputs
            * Slots - Specific for Intent of this interaction
            * Value - Input from users utterance. If user said the particular slot key.
        
        * Settings - Visitor Settings the tenant created, or saved from the `Save Settings` Component
        * Connectors - Integration, third party data sources
            * c1 - Specific connector created from the Connector Components
                * First - First item from list
                * Last - Last item from list
                * Length - Length of list

        * Var - variables created from `Add Variables` Component
        * Function
            * Array
                * random - picks a random item from the Array

            * Date
                * dateGet - gets the data from a specified variable
                * dateSet - sets specified date to a variable
                * now - return current date 
                * toRange - creates a date range from a date string

            * Geospatial
                * getZipcode - retrieve a zip code metadata

            * Number
                * add
                * mod - returns the modulus
                * number - returns variable or value as number

#. Save
#. Save & Close
#. Cancel


    .. image:: ./images/variable_interaction.png


================
Edit Interaction
================

* Double click desired Interaction
* Once changes are made, Click `Save` or `Save and Close`

==================
Delete Interaction
==================

* Double click desired Interaction
* Click delete button in the bottom left corner
    * A toast will appear to verify you truly would like to delete Interaction

================================
Features Within Interaction Grid
================================

* Filter Interactions
    * Interaction Status
        * Click on buttons to the top left
            * All | Pending | Approved

    * Intents Filter
        * Click and down arrow-key to intent and hit `enter`
        * Type name of intent and hit `enter`

    * Search Bar
        * Type text to search response for a particular value

        .. image:: ./images/interaction_grid.png

