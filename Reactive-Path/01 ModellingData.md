# Modelling Data

### Entities:

- Business Concepts are modelled and referred as entities. An entity allows us to persist and access the needed information in outsystems application.

- DB entities can hold data that can be stored in, and then retrieved from the databse.
- Entites have attributes and might have relationships with each other.

    - Attributes are DB Columns.
    - Identifiers are Primary Keys.
    - Referential attribute is foreign key.
    - Records are rows of the data.
    - Can have indexes which are index of the database table.

- ID attribute is created at the time of creation of the entity and this ID attribute can be modified in the future.
- Each attribute needs to have basic data type defined.
- For each datatype outsystems has a default value.So, each attribute will have a default value.
- Entity actions are automatically created and cannot be modified.
- Have CRUD actions.

### Static Entities

Static entites are a special type of entity that allows us to create a predefined list of values.

- It acts like an enumeration.
- They have attributes and records.
- Records cannot be changed at the runtime.
- Can be changed in development phase only.
- Have only one entity action: Get entity action. (Read Only)
- Created with 4 attributes by default: ID, Label, Order, IsActive
- The Set of Records can be found under the Records folder.
