## Process
1. Take notes here throughout the workday
2. End of Day or beginning of next day, go through all notes and move them to a more permanent location
3. Don't just copy and paste, improve the note as you transcribe it to its new location


# Today's Notes 

## Code Review Notes


## Pair Programming Notes
- reference repo: poc-cursor-based-pagination
- two types of pagination: limit + offset and cursor
- limit + offset work well for tables with forward and back buttons
- cursor works better for infinite scroll

- Difference b/w console.log and using logger
- logger provides time, log level (info, error,etc), scope, etc. which console.log does not
- pass repo specific logger to repo for instance, so that logger is decoupled from the repo
- logger can pipe logs to external service/server. Extendable
- logger can do log level scoping which allows us to configure what happens to certain levels of logs separately
- What should I log?? There should be standards/rules to follow for this
   - Errors
   - Warnings
   - Info
     - Changes to db, persistence layer
     - More of an art, and also iterative
     - More info = easier to deug, but also don't want overload or expose P.I.I.

Pairing on program tracker tests refactor
- Array.from({ length: count}, (_, index) => {...  the underscore is a feeler, like a place holder that isn't used because we need to use the index but don't care about the value

- Injecting one domain/module into another e.g. users needs customer domain
- 

### Brandon
- Generics
- declarative:
- imperative:

- zod is lining up your runtime data with your application code (DTO's)

- DDD coding, starting with type definitions

- Gating:
- gate 0: assess business reqs
- gate 1: shaping, find alignment, high level docs (Noah involved)
- gate 2: think about implementation (closer to priming), how do I achieve (engineers in squad)

- Chapter 4 of 99 bottles:


- 7/9/25
- endpoint is application layer in onion
- repository is application layer in onion
- usecase is service layer in onion
- domain layer in onion exists inside of that, no files exist yet
- when PM is talking that is a good indication that it is something in your domain layer

- using TS system to build an entity
- distinguish differences between things within entity
- use that to write a zod validator

- async + await is only necessary when you need the resolution of a promise, but often you only need the promise itself e.g. in the repo layer

- 7/10/25
- SSH
- Github

## Planning Notes
- Following the product and engineering all hands where a demo was given on the 3 amigos model, Wataru immediately followed up in our squads channel about how we will adopt this model
- 

