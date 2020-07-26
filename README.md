# SimpleRESTWebService

Attached is a simple REST web service created as part of the 'Master Java Web Services and RESTful Api with Spring and Spring Boot' (Udemy course).

This project contains a number of packages that address a wide range of areas involved in the development of a REST Web Service API. The key areas addressed by this project include:

- hello_world package: Explored and implemented common REST endpoint annotations i.e GetMapping, PostMapping etc. Most importantly, the concept of internationalisation was explored through the endpoint @GetMapping(path="/hello-world-internalisation"). Depending on the 'Accept-language' passed as a header in Get Request, endpoint retrieved different reponses i.e. Bonjour returned for 'fr'. 

- exception package: REST Exception Controller created to handle and return specifc details when certain exceptions are thrown in application utilising various HTTP Statuses. For example, trying to retrieve a user with an invalid id, resulted in the throwing of a UserNotFoundException and the endpoint ultimately returned a Http Status of 'Not Found' with other details such as a timestamp and exception specific details. 

- filtering package: In depth look into filtering with Jackson. Namely, various fields filtered out before returning responses in GetMapping requests using MappingJacksonValue class. 

- versioning package: PersonV1 and PersonV2 classes created to mimic the versioning an api might go through. Various endpoints created in controller to explore different methods of maintaining old and new endpoints primarily using Content and Header Negotiation 

- Finally, basic Spring security was implemented using starter spring security. 

To test endpoints: select basic Auth for endpoints in Postman and Username is 'user' and password is default password printed in log on start up of application. 
