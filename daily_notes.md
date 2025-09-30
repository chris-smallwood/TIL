# Place to take notes daily

## End day by transcribing notes from here to specific documents. Goal of reinforcing learning and organization.

### EXP - Present

#### Internet - How does the internet work? - How does the internet work? whitepaper
- ping <domain name> command in terminal
- each message sent across internet broken into packets
- traceroute <domain name> command in terminal


### Code Review
#### https://github.com/routeware/engagement-programtracker/pull/52
- **Array.isArray(res) ? res.length > 0 : !!res;**
  - Is res an array? yes, case 1. no, case 2
  - Case 1: If res is an array, does it have elements? yes, true. no, false
  - Case 2: If res is not an array, convert res to a boolean.
    - **!!null** and **!!undefined** return false
    - **!!{}** and **!!"string"** return true
  - **!!value** in TS/JS converts any value to its boolean equivalent
    - equivalent to **Boolean(value)** and **res ? true : false** but is the common preference for readability and performance
   
`export function createService(dependencies: { notifier: Notifier; logger: PTLogger }): 
{ exposedFunction: customTypeOfExposedFunction } {
  return { exposedFunction: (exposedFunctionParams) => { ...exposedFunction definition. probably use dependencies? } }`
  - classic factory function pattern
    - encapsulates the Service's logic
    - allows dependency injection (testing and flexibility)
    - returns a clean API with just exposedFunction exposed outside of the factory
    - performs but hides all internal implementation details of the service


### Wataru Pairing
- write tests against our code, not a library being used
- 
