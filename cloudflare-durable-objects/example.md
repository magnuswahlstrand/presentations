|           | Workers | Durable<br>Objects |
|-----------|---------|--------------------|
| Execution |         | Single-threaded    |
| Use cases |         | aa,<br>aa          |

---


```javascript [|3|7|11]
async function fetch(request, env, ctx): Promise<Response> {
    // This id refers to a unique instance of our 'MyDurableObject' class above
    let id: DurableObjectId = env.MY_DURABLE_OBJECT.idFromName('magnus');

    // This stub creates a communication channel with the Durable Object instance
    // The Durable Object constructor will be invoked upon the first call for a given id
    let stub = env.MY_DURABLE_OBJECT.get(id);

    // We call the `sayHello()` RPC method on the stub to invoke the method on the remote
    // Durable Object instance
    let greeting = await stub.getCounter();

    return new Response(greeting);
}
```