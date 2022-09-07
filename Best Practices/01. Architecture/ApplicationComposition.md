# The 4 Rules for Correct Application Composition


Rules are made in order to:
1. Minimize Dependencies
2. Simplify Deployments
3. Promote life ccle independence.


# Rule #1 - Correctly layer your modules

# Rule #2 - Correctly layer your applications

# Rule #3 - Don’t mix different owners

- Having more than one owner for an application results in complex deployment management, as accountability for what has been changed becomes unclear.


# Rule #4 - Don’t mix different sponsors
- If a project affects several sponsors, it's important to isolate each LOB (Line Of Business) in a different application. Different sponsors have different budgets, requirements and change paces.

- Splitting the application upfront, by LOB, enables the independent evolution of each one. The isolation of all the common services clearly sets the border between what must be carefully planned due to the expected transversal impact, and what can be flexibly changed inside each LOB.