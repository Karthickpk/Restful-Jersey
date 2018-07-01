# Restful Jersey

REST Overview
REST was built with the pains of SOAP in mind
Built on the principles of HTTP
Services can return :
•	XML
•	JSON
•	HTML
•	Plain Text
•	Binary/octet

HTTP GET Request [GET] :
•	Annotated with @GET
•	Mapping is de!ned with @Path
•	The URL is de!ned through our context/servlet mapping/@Path
•	Content returned is de!ned with @Produces
	 @Produces can take an Array of multiple types