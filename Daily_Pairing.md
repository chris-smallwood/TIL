node -e 

agents.md in repo to direct ai agent

post-customer.ts -> zod validator
create-customer.ts -> CreateCustomerProps

These are both parts of the domain and should be tied (ez.infer typeof). Incurring cost by maintaining them separately

Generally, where can I put concepts so that I only have to change it once and the change propogates on its own


        //http layer
        if (ts result == negative){
          ctx.message = result.message;
          // ctx.status = statusEnum.get(result.message);
         ctx.status =  httpCodeFor(result.code);
        }

Endpoint (API layer) is just interface for outside (front end client) so protects from anonymous users
Usecase (domain layer) is interface for other developers (e.g. cli) so protects database
Many things could be validated
