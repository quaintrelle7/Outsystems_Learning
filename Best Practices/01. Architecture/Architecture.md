The Architecture Canvas is an OutSystems architecture tool to make the design of Service-Oriented Architectures (SOA) simple. It promotes the correct abstraction of reusable (micro)services and the correct isolation of distinct functional modules, in cases where you are developing and maintaining multiple applications that reuse common modules.


#### Benefit
> The most important benefit you get out of a well designed architecture is that applications and the modules that compose them will preserve independent lifecycles and decrease to a minimum dependencies and overall change impact.

## The layers

End-User

Core Modules

Foundation Modules


# Validating your application architecture


- It analyzes the actual dependencies among modules, identifying violations and pinpointing the elements (actions, screens, entities) that are assembled in the wrong place.

## Rule 1 - No upward references

> An upward reference tends to create a cluster where any 2 modules, directly or indirectly, have a circular dependency.

- An upward violation clearly identifies that services are not properly isolated.

### How to fix?

- Move the elements that are being consumed to the lower layer.

## Rule 2 No side references among End-users or Orchestrations

> End-user or Orchestration modules should not provide reusable services. This ensures that they are correctly isolated, allowing them to have different lifecycles - different versioning paces due to different sponsors or project teams.

- A reference to suchs modules tends to bring along a huge set of indirect dependencies from lower layers.

### How to fix?

- Find out which are the elements of B being consumed by A and move them to a new (or an existing, if there is a conceptual fit) lower layer module:
    To a Core module if it is business related.

    To a Library if it is business-agnostic.



## Rule 3 - No cycles among Cores or Libraries

- The third rule is about avoiding cycles among Cores or Libraries, since those are allowed to have side references.

- A cycle between modules indicates that the concepts are not correctly abstracted.

> A cycle between A and B either indicates that:

    - They are strongly coupled, or;

    - One of the directions is undesirable. For instance, A should be conceptually consuming B because the concept in A extends B.

### How to fix?

- Most of the times, if there is clearly an undesirable direction in the relation concepts must be moved to another module.

- For example, if it is B that should not be consuming A, then the elements of A consumed by B should be:

- Moved to a new module, if they represent another reusable concept, or;

- Moved to B itself, if they were misplaced elements of the same concept.

- However, If A and B are too strongly coupled, they should be merged together