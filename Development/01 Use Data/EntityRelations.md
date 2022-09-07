> Relationships are created by defining a single reference attribute. 

## One-to-One



## Referential Integrity

> When you create relationships between an entity A and an entity B, you must specify the referential integrity mechanism that you want to apply in your module, i.e. what must happen in entity B if the corresponding record in entity A is deleted. 

## Relationship Indexes

- When the reference attribute is defined, an index is automatically created in order to improve the performance of your module. This index is called:

- AutoIndex_<reference attribute name>

and covers the reference attribute that implements the relationship.

You should not delete this index. 