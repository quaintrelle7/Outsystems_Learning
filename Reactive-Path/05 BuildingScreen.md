# Fetching Data

https://success.outsystems.com/Documentation/11/Developing_an_Application/Implement_Application_Logic/Screen_and_Block_Lifecycle_Events

## 1) Using Screen Aggregates
    - Using Screen Aggregates within screen scope only.


## 2) Through Data Actions
    - Define server-side logic inside data actions.
    - Allow calling external REST web services.
    - Or executing advanced SQL queries.
    - Outputs of these data actions can be used in the screen widgets.


Data Actions and Aggragtes are triggered automatically, they executes on screen initialization.

- Both of them run asynchronously, so when they are more they run in parallel.

- When Aggragate or Data Actions finishes the execution, the screen renders automatically and displays the returned data.

- With multiple aggragtes and actions this happen everytime new data is available.

- Widgets source property expects a list to display.
