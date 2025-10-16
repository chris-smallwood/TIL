
AKA Ports and Adapters

Goal: decouple domain logic (business rules) from external concerns like db, API's, UI's

Result: maintainable, testable, scalable backends

Components:
- Domain (core application): pure business logic and use cases
- Ports: interfaces defining how external components interact with domain
  - specifies the language that is allowed to communicate with the hexagon (core).
- Adapters: implementations of port interfaces that allow external tools to connect to domain
  - serve to convert the language of the actors into the language understood by the hexagon, specified by the port

Uses:
- Dependency Injection: inject adpaters into your use cases to enhance testability
- Dependency Inversion: when establishing dependency for a protocol structure, INVERT the dependency of that object for anotherconcrete object
- Single Responsibility Principle (SRP): each function should have one job
- Configurable Dependency: dependency of an object (or function) on an interface (or protocol)

Results:
- Infrastructure Agnostic: core should not depend on external libraries or frameworks... implementation details
- domain logic knows nothing external to it, everything external managed via adapters

Questions:
- adapters can import ports (interfaces), core service implements a port (interface)?
