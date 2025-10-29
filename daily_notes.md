# Place to take notes daily

## End day by transcribing notes from here to specific documents. Goal of reinforcing learning and organization.

### EXP - Present

#### Hexagonal Architecture
https://jmgarridopaz.github.io/content/hexagonalarchitecture.html#tc3

###### Intro
1. Promotes decoupling from technology (libraries)
2. Defines structure of the application so that it can be run by different kinds of clients and tested in isolation from external devices

###### Architecture
1. Hexagon is the application itself (core, domain?)
2. Ports are interfaces, boundary of the hexagon
3. Ports belong to the application (hexagon)
4. Adapters are components that allow a technology to interact with a port
5. Adapters convert a specific technology request into a technology-agnostic request to the port
6. For each driver port, there should be at least two adapters: one for the real driver that is going to run it, and another one for testing the behaviour of the port
7. Main job of an adapter is to convert one interface into another (Adapter Design Pattern)
8. Composition Root (from Martin's Clean Architecture) return to this for implementation

###### Configurable Dependency Pattern
1. Generalizes dependency injection, (sometimes called inversion of control)
2. Dependency injection is the thing you do to achieve this pattern
3. Configurable dependency is the dependency of an object on an interface
4. Interface is a parameter of object constructor (OOP, param of builder in functional). At runtime, a specific implementation of the interface is passed during instantiation.
5. This pattern is integral to Ports & Adapters. It is how the hexagon is decoupled.
6. Configurable Dependency implementation is different for each side. In the driver side, the application doesn’t know about which adapter is driving it. But in the driven side, the application must know which driven adapter it must talk to.
7. 







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
 

