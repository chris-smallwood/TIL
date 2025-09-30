

`export function createService(dependencies: { notifier: Notifier; logger: PTLogger }): 
{ exposedFunction: customTypeOfExposedFunction } {
  return { exposedFunction: (exposedFunctionParams) => { ...exposedFunction definition. probably use dependencies? } }`
  - classic factory function pattern
    - encapsulates the Service's logic
    - allows dependency injection (testing and flexibility)
    - returns a clean API with just exposedFunction exposed outside of the factory
    - performs but hides all internal implementation details of the service
