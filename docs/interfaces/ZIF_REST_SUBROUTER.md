# Subrouter Interface
- The Router uses this interface to find route using specific method.
- Classes defined using this interface have only one role and that is to find specific route for given URI. 
- It does not concern itself with object creation.
- It uses Helper class for database operations
## Methods
### FIND_ROUTE
- Finds route from given URI
Parameters: <br>

| Parameter   | Type | Typing Method | As. Type               | Description                 | Other | 
| :---------- | :--: | :------------ | :--------------------- | :-------------------------- | :---- | 
| IO_HELPER   | Imp. | Type Ref To   | ZIF_REST_ROUTER_HELPER | Interface For Router Helper |       | 
| IV_PATH     | Imp. | Type          | STRING                 | URI Path                    |       | 
| ET_VALUES   | Exp. | Type          | ZTT_URI_VALUE          | Table Type For URI Values   |       | 
| RV_ENDPOINT | Ret. | Type          | ZDE_SERVICE_ENDPOINT   | Endpoint For Rest Service   | Value | 

Exceptions: <br>
ZCX_ST_REST_SERVER_FAIL

## Attributes

| Attribute         | Level    | Typing Method | As. Type | Description             | Other | 
| :---------------- | :------- | :------------ | :------- | :---------------------- | :---- |
| CO_ROUTER_TYPES   | Constant | Structure     |          | Router Types Constant   |       |
| CO_ROUTER_CLASSES | Constant | Structure     |          | Router Classes Constant |       |

## Stuctures
### CO_ROUTER_TYPES

| Name  | Typing Method | As. Type        | Value   | 
| :---- | :------------ | :-------------- | :------ |
| smart | Type          | ZDE_ROUTER_TYPE |	'SMART' |

### CO_ROUTER_CLASSES

| Name  | Typing Method | As. Type  | Value                      | 
| :---- | :------------ | :-------- | :------------------------- |
| smart | Type          | CLASSNAME | 'ZCL_REST_SUBROUTER_SMART' |