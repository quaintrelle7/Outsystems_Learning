# Logic Actions

> An Action is an element that allows us to define logic flows on the server and client side.


- An Action flow can have onlu one start node and multiple end nodes.
 - Destination End (Screen Actions Only)
 - Download End (Screen Actions Only)

## Three Types of Actions:

### 1) Screen Actions
 - Defined inside a screen.
 - Bound to the widgets that are part of the screen.
 - Scope includes screen level only.
 - Such as aggregates, widgets, variables.
 - Execute on the browser.
 - Doesn't have output parameters.
 - Can use screen actions from within same screen, but not from another.
 - Can call other client actions.
 - Created under Interface tab.

### 2) Client Actions
 - Used throughout the module and are not bound.
 - Execute on the browser.
 - Can have input params, local vars and output params.
 - Can call other client actions.
 - Created under logic tab.

### 3) Server Actions

 - Defines logic to be executed on server-side.
 - Can have input params, local vars and output params.
 - Can call itself and other server actions.
 - Created under logic tab.

> Both Client and Server Actions can be set as a function. Then they can have only one parameter and can be used inside the expressions.

## Code Reusability

- It means logical code reusability.
- Reusable logic is provided through actions.


# Variables

