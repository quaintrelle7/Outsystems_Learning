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




# Site Properties

    Site Property is a global configuration variable that stores application-wide information.

- Can be used to store settings for app, and its value is shares by all end-users on the environment.
- They exist on the SERVER-SIDE ONLY.   
- They can store the basic data types only, such as integers, text values and entity identifiers.
- Value can be changed at the runtime. Without Service Studio, through Service Center.
- Value is environment-specific. This means development and production may have completely different values.

## Usage of Site properties

- To store an API Key for a remote web service.
    - As different API keys may be set in dev and prod.
- To enable or disable a new application feature.

> Site Properties should not be used for the values that change often. Should be considered as constants.