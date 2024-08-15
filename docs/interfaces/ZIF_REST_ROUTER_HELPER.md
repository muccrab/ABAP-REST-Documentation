# Router Helper Interface
- This interface provides methods, that enable classes on the Router Layer to obtain information from the database
- Only classes that have this interface should be working with Customizng Layer data.

## Methods
### GET_ENDPOINT_ROUTES
- Get All Endpoint Routes
Parameters: <br>

| Parameter   | Type | Typing Method | As. Type               | Description                       | Other | 
| :---------- | :--: | :------------ | :--------------------- | :-------------------------------- | :---- | 
| RT_RESULT   | Ret. | Type          | TT_ROUTES              | Table Of Possible Endpoint Routes | Value | 



### GET_SERVICE
- Get Service Name
Parameters: <br>

| Parameter   | Type | Typing Method | As. Type               | Description                 | Other | 
| :---------- | :--: | :------------ | :--------------------- | :-------------------------- | :---- | 
| RV_RESULT   | Ret. | Type          | ZIF_REST_ROUTER_HELPER | Name of Rest Service        | Value | 

### GET_METHOD
- Get Rest Method For Endpoint
Parameters: <br>

| Parameter   | Type | Typing Method | As. Type               | Description                 | Other | 
| :---------- | :--: | :------------ | :--------------------- | :-------------------------- | :---- | 
| RV_RESULT   | Imp. | Type          | ZDE_REST_METHOD        | Rest Method                 | Value | 

### GET_SECURITY
- Get Name of the Security Class
Parameters: <br>

| Parameter   | Type | Typing Method | As. Type               | Description                 | Other | 
| :---------- | :--: | :------------ | :--------------------- | :-------------------------- | :---- | 
| IV_ENDPOINT | Imp. | Type          | ZDE_SERVICE_ENDPOINT   | Endpoint For A Service      |       | 
| RV_SECURITY | Imp. | Type          | CLASSNAME              | Security Class Name         |       | 

### GET_DESTINATION_FOR_ENDPOINT
- Get Destination For the Endpoint
Parameters: <br>

| Parameter      | Type | Typing Method | As. Type               | Description                 | Other | 
| :------------- | :--: | :------------ | :--------------------- | :-------------------------- | :---- | 
| IV_ENDPOINT    | Imp. | Type          | ZDE_SERVICE_ENDPOINT   | Endpoint For A Service      |       | 
| RV_DESTINATION | Ret. | Type          | CLASSNAME              | Endpoint Class Name         | Value | 

Exceptions: <br>
ZCX_ST_REST_SERVER_FAIL

### GET_SUBROUTER_CLASS
- Get Name of the Subrouter Class
Parameters: <br>

| Parameter    | Type | Typing Method | As. Type  | Description                 | Other | 
| :----------- | :--: | :------------ | :-------- | :-------------------------- | :---- | 
| RV_SUBROUTER | Ret. | Type          | CLASSNAME | Subrouter Class Name        |       | 

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