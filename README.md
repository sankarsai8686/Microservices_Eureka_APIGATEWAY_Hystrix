# Microservices_Eureka_APIGATEWAY_Hystrix
Microservices_Eureka_APIGATEWAY_Hystrix
MicroServices_2Services_EurekaServiceRegistry_API_GATEWAY_Hystrix&BashBoard_CloudConfig



Created 2 individual Services
For Communication two services used RESTTEMPLATE.
To Remove hardcoding IP&PORTS, Introduced EUREKA REGISTRY SERVER. And those 2 services now with register with Eureka as a client
Introduces API GATEWAY, so that client can able to communicate directly with API GATEWAY, now out side people don't know in which port those services running. API GATEWAY will Identify request with the help of filters and same forward to respective servers.
For Handling Fallback or Connection timeout while connecting with servers, introduced hystrix & hystrix dashboard so we can send appropiate message to client.
Introduced Cloud Config to keep common properties among all services in a git same will configured in cloud server, this same will now will use all other services, example commom properties are eureka server config.
