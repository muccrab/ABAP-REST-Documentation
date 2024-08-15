# Customizing Table For Endpoint Management
 - In this table user can setup endpoints for their services
 - It has one foreign key *SERV* with header table [ZCT_SERVICE](/tables/ZCT_SERVICE). 

## Mainteinance View
*ZMV_ENDPOINT*

## Fields

| Field           | KEY | Not NULL | Data Element         | Data Type | Description            | 
| :-------------- | :-: | :------- | :------------------- | :-------- | :--------------------- | 
| MANDT           | KEY | Not NULL | MANDT                | CLNT(3)   | Client                 | 
| SERV            | KEY | Not NULL | ZDE_SERVICE_NAME     | CHAR(20)  | Name of Rest Service   | 
| REST_METHOD     | KEY | Not NULL | ZDE_REST_METHOD      | CHAR(10)  | Rest Method            | 
| ENDPOINT        | KEY | Not NULL | ZDE_SERVICE_ENDPOINT | CHAR(150) | Endpoint For A Service | 
| INTERFACE_CLASS |     | Not NULL | CLASSNAME            | CHAR(30)  | Reference type         | 
| SECURITY_CLASS  |     |          | CLASSNAME            | CHAR(30)  | Reference type         | 
