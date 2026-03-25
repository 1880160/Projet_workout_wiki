# Design Patterns used across the project

## Composite
The composite pattern will be used to structure our routes. Therefore, subroutes will be contained within subfolders in a structure similar to the api/frontend's routes. 

## Singleton
NestJs uses singleton by default in its' repository.


## Decorator
Decorator will be used to inject code within function and routes
to greatly reduce code amount and increase code readability.

## Observer
The server will use SSE(Server Side Events) to notify the client of real time notification such as workout alerts and exercise review request.
