# Generic Rest Router Class
Redirects the traffic to the correct endpoint
## Interfaces
IF_REST_HANDLER
## Methods
### IF_REST_HANDLER~HANDLE
Processes a REST Request<br>

| Parameter  | Type | Typing Method | As. Type          | Description   | Other | 
| :--------- | :--: | :------------ | :---------------- | :------------ | :---- | 
| IO_REQUEST | Imp  | Type Ref To   | IF_REST_REQUEST   | REST Request  |       | 
| IO_RESPONSE| Imp  | Type Ref To   | IF_REST_RESPONSE  | REST Response |       | 
| IO_CONTEXT | Imp  | Type Ref To   | IF_REST_CONTEXT   | REST Response |       | 