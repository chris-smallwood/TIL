
0. Ideally event storming preceedes this and identifies an aggregate or atleast an entity to start this next process
1. Define route
2. Ask... what is a route
3. Define some attributes of a route
4. Have conversation about attributes which should reveal business rules and ubiquitous language
5. Define attributes in terms of primitives
6. Codify primitives (we use zod and then derive types from zod objects)
7. Above results in very solid shared understanding of a route between PM and Dev

This model supports:
- pipelines in the usecases resulting in code that is easier to understand and debug
- dependency injection (in order to build pipelines)
- separation of concerns

Tip: usually easier to compose small units into a larger one than decompose a larger one into smaller units.
More downstream consequences in your code base when decomposing vs composing

pipeline operator in TS (coming out in future version of TS): step1 |> step2 |> step3
