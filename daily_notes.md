# Place to take notes daily

## End day by transcribing notes from here to specific documents. Goal of reinforcing learning and organization.

### EXP - Present

#### Hexagonal Architecture
- AKA ports and adapters
- Goal: decouple domain logic (business rules) from external concerns like db, API's, UI's
  - result: maintainable, testable, scalable
- domain logic knows nothing external to it, everything external managed via adapters
- Components:
  - Domain (core application): pure business logic and use cases
  - Ports: interfaces defining how external components interact with domain
  - Adapters: implementations of port interfaces that allow external tools to connect to domain
- Dependency Injection: inject adpaters into your use cases to enhance testability
- Single Responsibility Principle (SRP): each function should have one job
- Infrastructure Agnostic: core should not depend on external libraries or frameworks... implementation details
- Chris: adapters can import ports (interfaces), core service implements a port (interface)

- Configurable Dependency: dependency of an object (or function) on an interface (or protocol)
- when establishing dependency for a protocol structure, INVERT the dependency of that object for anotherconcrete object
- The port specifies the language that is allowed to communicate with the hexagon (core). The adapters serve to convert the language of the actors into the language understood by the hexagon, specified by the port
- 

#### HTTP - videos
- TLS

### Code Review
#### https://github.com/


#### Pagination Utility

   
### Brandon Pairing

RAY-977
- 

- checkout tsconfig.json
- parse vs safeParsej
- types vs interfaces

- TS Result ```ts-resuls-es``` for implementing step result functionality


### Wataru Pairing
 

