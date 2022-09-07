# Architecture design process

### Disclose
business concepts and integration needs

- Functional Requirements
- Non Functional Requirements




### Organize
concepts on the architecture Layer canvas

1. End User Layer:
	User interfaces and processes, reusing Core and Library to implement the user stories.
2. Core layer:
	Services around business concepts, exporting reusable entities, business rules, and business widgets.
3. Foundation Layer:
	Business-agnostic services to extend the framework with highly reusable assets, UI Patterns, connectors to external systems, and integration of native code.

### Assemble
Matching recommended patterns

- Join concepts if they're conceptually related.
- Don't join concepts if they're too complex or have different life cycles.
- Isolate the reusable logic from all the integration logic that consumers don't care about.
