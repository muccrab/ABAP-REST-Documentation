# Security Wrapper Interface
- Security Wrapper For specific Endpoints.
- By Extending this interface you can create new security classes.
- The security can be either specific for endpoints, or/and the service.
- If security is defined on endpoint, it will be used, otherwise the security of service will be used.
- There is predefined class <b>ZCL_REST_SECURITY_NONE</b>, that is used when no security is defined.
- The security is then run in the <b>RUN_SERVICE</b> method
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

## Attributes
| Attribute   | Level    | Typing Method | As. Type    | Description               | Other | 
| :---------- | :------- | :------------ | :---------- | :------------------------ | :---- |
| IO_REQUEST  | Instance | Type Ref To   | IF_ENDPOINT | Endpoint For Rest Service |       |