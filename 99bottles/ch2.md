

## Review w/ Brandon

### TDD
- Tests should not mirror implementation!
- The point of an object or function is to encapsulate logic
- Tests should be written so that they have no knowledge of how an object or function does what it does.
- ONLY KNOWS INPUTS AND OUTPUTS. no knowledge of internals of what you are testing
- If a test mimics implementation of a function, then you have to refactor the test when you refactor the code. Now the test is ineffective.
- Tests should remain stagnant when refactoring code

### DDD
- Usecases are what meet your business requirement.
- Units are used to build up your usecase
- Units that are not being used for a usecase probably have no purpose in your application, delete!

### Code Review
- in users endpoints, customer_id shows up in validate const in multiple endpoints
- this can be pulled into domain specific files that define your validators and types for the domain
- DRY out your usecases

### Career
- code review is learning what not to do
- planning and mentoring is learning what to do
- GITHUB COPILOT (usage being monitored)
- smaller units of work, more frequent feedback
- figuring out the smallest unit of work is feasible for a single ticket requires some planning and foresight
- signal your intent, this is what I'm aiming for in this PR AND here's what I didn't do
- it is OK to not consider certain things

- Muy thai kicking example
- Start by kicking the pad
- Next try implementing one improvement on that movement
- Repeat until you can succeed at that
- Move on to the next improvement

- One style of mentorship is to outline and teach all of the steps ahead of time and let the student actively participate in choosing which step(s) to focus on next
- Another style is to only reveal the next chosen step work on when the mentor believes the student is ready to focus on that next step

- Also don't wait too long to start implementing the next step.
- If it has become glaringly obvious what you need to do, then it is time to start practicing the next step.
- Motivation: tech debt has compounding interest AND orgs do not prioritize refactoring.
