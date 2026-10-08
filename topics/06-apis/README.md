# APIs and Software Interfaces
## Core idea
An API (Application Programming Interface) defines how software components interact: which operations exist, what inputs they accept, what outputs they produce, and how failures are reported.

An API does not have to use the internet. A library function, an operating-system call, and a web endpoint can all expose APIs.

## Example contract
A hypothetical task service exposes:
```http
GET /tasks/42
```
A successful response could contain:
```json
{"id": 42, "title": "Study heaps", "completed": false}
```
The contract should also define what happens when task 42 does not exist, who may read it, and which fields are stable.

## Terms that are easy to confuse
- **Endpoint:** a particular access point, often described by an HTTP method and path.
- **Library:** reusable code called by your program.
- **SDK:** tools and libraries intended to help develop for a platform or service.
- **REST:** an architectural style with constraints, including stateless interactions and a uniform interface. Returning JSON alone does not make an API RESTful.
- **Authentication:** establishes identity.
- **Authorization:** determines permitted actions.

## Why it matters
Consumers depend on contracts. Renaming a response field or changing its type may break clients even if the server still runs.

## Try it
Design the inputs, successful response, and two failure cases for “create a task.” Decide which fields the client supplies and which the server generates.

## Expand next
Request validation; pagination; idempotency; rate limits; API versioning; webhooks; REST, RPC, and GraphQL.

[Back to index](../../README.md)
