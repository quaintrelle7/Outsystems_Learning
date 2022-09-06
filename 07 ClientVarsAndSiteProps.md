# Client Variables

    Client vars allows to store long lived and user specific configurations.

    - Values stored on these vars are user specific.
    - Values are restricted to basic data types and entity identifiers.
    - Client Browser stores all Client Variables. On log out client variables are reset to their default.
    - Closing the browser will not cause the loss of the client variable values.
    - The browser stores the values and re-loads them whenver it's opened again.

## Usage of Client Variables

    - To store cache info like username, that may save few requests to the server and databse.
    - To store configuration or settings for the user. Like the search keyword in list screen.
    - Or layout.

    