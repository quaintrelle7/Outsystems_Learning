# Session Variables


> In OutSystems, a Session is created in the first request the end user makes to the Platform Server and allows to keep context during the end user interactions with the server. The session consists in the set of session variables defined in the modules the end user accesses during its interaction. The session variables can be used when you are implementing the business logic of your module, for example, in user-actions, screen preparations, and screen actions.

Session variables hold data that is persisted during the session and can be used to save information during the end user interaction. Each application has several session variables automatically created, but you can define new ones.

The session variables are initiated automatically by Service Studio when the Platform Server session is created. While the session exists, you can use these variables in your business logic. When the session ends, the session variables are set to their default value.


## Examples


Username
- This variable is instantiated during the login operation, whether you are using an explicit or implicit login. At logout, this session variable is assigned an empty text value.

- When the end user logs in or out, using the Login, LoginPassword, or Logout actions, the user-defined session variables are set to their default value.


# Caching

These are the elements that support caching:

- The lists returned by Aggregate and SQL.
- Output parameters of custom Server Actions.
- Web Blocks and elements they contain (Traditional Web Apps only).

Some elements don't support caching. These are:

- Screens, as the feature currently does not support this element.
- Exposed REST
- Web Blocks with Submit or Ajax Submit.