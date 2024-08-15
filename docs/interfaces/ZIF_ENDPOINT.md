# Endpoint Interface
- Interface For user definable endpoint classes.
- By Extending this interface you can create new endpoints.
- The endpoint is then run in the <b>RUN_SERVICE</b> method
## Methods
### RUN_SERVICE
Parameters: <br>

| Parameter   | Type | Typing Method | As. Type          | Description   | Other    | 
| :---------- | :--: | :------------ | :---------------- | :------------ | :------- | 
| IO_REQUEST  | Imp. | Type Ref To   | IF_REST_REQUEST   | REST Request  |          | 
| IO_RESPONSE | Imp. | Type Ref To   | IF_REST_RESPONSE  | REST Response |          | 
| IO_CONTEXT  | Imp. | Type Ref To   | IF_REST_CONTEXT   | REST Context  |          | 
| IO_VALUES   | Imp. | Type          | ZTT_URI_VALUE     | Rest Method   | Optional | 

Exceptions: <br>
ZCX_ST_REST_SERVER_FAIL
