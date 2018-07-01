# Restful Jersey

> REST Overview
REST was built with the pains of SOAP in mind
Built on the principles of HTTP
Services can return :
- XML
- JSON
- HTML
- Plain Text
- Binary/octet

> HTTP [GET] Request
- Annotated with @GET
- Mapping is defined with @Path
- The URL is defined through our context/servlet mapping/@Path
- Content returned is defined with @Produces
	- @Produces can take an Array of multiple types
	
> HTTP [PUT] Request
- Early on some browsers didn’t support PUT (or DELETE)
- REST often gets over simplified
	- Developers use POST to CREATE and UPDATE
	- Theoretically PUT can be used for both functions
- PUT is idempotent
	- We can call PUT multiple times and it shouldn’t affect the app
	- Think of it like a SQL update, we can update the database multiple times and 	it won’t affect the app
	- PUT should be used if you are supplying the ID for your Object
	- POST should be use if the server is supplying the 
	
> HTTP [DELETE] Request
- Like PUT, early browsers didn’t support DELETE
- Deletes are to a specific URL
	- http://localhost:8083/exercise-services/webapi/activities/1234
- Deletes can be recursive too
	- http://localhost:8083/exercise-services/webapi/activities
	- Careful! This would delete all activities
- Also like PUT, DELETE is idempotent
	- Calling delete multiple times on a url shouldn’t matter

> RESTFul Searching
- Simple and easy to use
- Typically used with GET
	- http://localhost:8083/exercise-services/webapi/activities?duration=55&description=swimming
- Cacheable since it is a GET

> RESTFul Searching Ranges
- For simple cases
	- from QueryParam
	- to QueryParam
- http://localhost:8083/exercise-services/webapi/activities?durationFrom=30&durationTo=60
- Very limited, but still works
	
	
by Karthick Kalimuthu :simple_smile: :+1: