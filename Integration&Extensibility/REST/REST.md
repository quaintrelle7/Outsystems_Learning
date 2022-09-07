# Consume REST APIs

- To retrieve or manipulate information from another system. Consume REST API.


## REST API Authentication

####  Basic Authentication 

- Consume REST API in system

#### Token Based Authentication

- use the "OnBeforeRequest" callback to add the required HTTP authorization header to the outgoing requests.

#### Cient certificate authentication

- use the "OnBeforeRequestAdvanced" callback, together with .NET code in an extension, to customize the outgoing requests. 

## REST API Structures

When you consume REST API methods in your module, OutSystems automatically creates the Structures that define the information held by the input and output parameters. The name of each Structure is generated from:


- The HTTP Request type
- The method name
- If it will hold a Request or a Response


# Expose REST APIs


## REST API METHOD FLOW


1) Security Validations
    - OutSystems executes the security validations according to the settings in REST API properties HTTP Security and Internal Access Only.


2) OnRequest()
    - OnRequest callback allows you to run logic over the requests after receiving them.


3) OnAuthentication()

    - OnAuthentication callback allows you to add basic authentication or custom authentication to requests.

4) Parameters Deserialization and Validation
    - Deserialization of the input parameters and validation of the data types, mandatory values, etc.

5) Method Execution
    - Executes the action that implements the REST API Method.

6) Parameters Serialization
    - Serialization of the output parameters to return in the response.

7) OnResponse()
    - OnResponse callback allows you to run logic over the responses before sending them. It is always executed, even in an error situation.


