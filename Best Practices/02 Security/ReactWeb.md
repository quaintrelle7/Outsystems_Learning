# Client-side security


    A rule of thumb for client-side security is that the code that is on the client-side and can be used by the end-user via its unauthorized modification which can result in changes in content or behavior of your application.
    
https://success.outsystems.com/Documentation/Best_Practices/Security/Reactive_web_security_best_practices

## Don’t expose sensitive data on the client-side

## Retrieve only the necessary data for the screen

## Securing server calls

## Protect screens and aggregates with roles

## Securing user accounts on Public screens interactions


# Server-side security

## Validate security in core modules

- Start an action with User and Roles validations on by using GetUserId() and Check<RoleName>Role(), to see if this user is allowed to execute this action.



- Don’t deploy test screens to other environments than the development environment. They are normally Public screens with quite some functionality which you can use to tamper with the database.

- Keep track of the 3rd party plugins you are using. They can also contain vulnerabilities. When you don’t check regularly or update the components on a regular basis, you have the chance to get attacked via known vulnerabilities.