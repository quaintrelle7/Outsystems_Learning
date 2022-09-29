01. Opening an application
- Screen is loaded
- Dsiplays configured splash screen
- Navigates to defualt screen

02. Displaying Splash scree
- Check the user role against the roles with permission to access the screen
- OnInitialize is Triggered.
    Dom is not comepltely loaded when this event occurs. Can use this event handler to implement all logic that doesn't require the DOM.

03. After end of OnInitialize event handler
- Aggregates and data actions of the default screen start to fetch data.
- DOM loads Ready and Render event handlers.

Ready event only happens when opening the screen.

Render event havveps every time the data of the screen is modified.

04. Navigating between screens

- When navigation starts, the DOM of the target screen immediately starts to load.
- DOM of the old screen is removed only after the Render event of the target screen.
- After the Render event of the target screen, the transition between the screens happens and the older screen is finally removed from the DOM.
- DOM fo the both screens are available between the target screen and the Destroy event of the od screen.


05. On Changing the Data of the


Render and refreshes the data.