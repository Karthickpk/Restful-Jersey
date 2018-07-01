# Restful Jersey

REST Overview
REST was built with the pains of SOAP in mind
Built on the principles of HTTP
Services can return :
- XML
- JSON
- HTML
- Plain Text
- Binary/octet

> myresource
HTTP GET Request [GET] :
- Annotated with @GET
- Mapping is defined with @Path
- The URL is defined through our context/servlet mapping/@Path
- Content returned is defined with @Produces
	- @Produces can take an Array of multiple types