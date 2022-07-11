# task001
DIFFRENCE BETWEEN HTTP/1.1 & HTTP/2

HTTP-hypertext transfer protocol & it is used in client-server communication.
By using HTTP user sends the request to the server & the server sends the response to the user.

HTTP/1.1: When you make a request to the server for a html page & server responds to you as a resource of that html page.
before sending the request and the response there is a TCP connection established between client & server.again you make a 
request to the server for image img.jpg & the server gives a response as an image img.jpg. the connection was not lost here 
after the first request because we add a keep-alive header which is the part of the request so there is an open connection 
between the server & client.there is a persistent connection which means several requests & responses are merged in a single connection.
These are the drawbacks that lead to the creation of HTTP/2: The first problem is HTTP/1.1 transfer all the requests & responses 
in the plain text message form.The second one is head of line blocking in which TCP connection is blocked all other requests until
the response does not receive. all the information related to the header file is repeated in every request.

HTTP/2: HTTP/2 was developed over the SPDY protocol. HTTP/2 works on the binary framing layer instead of textual 
that converts all the messages in binary format. it works on fully multiplexed that is one TCP connection is used 
for multiple requests. HTTP/2 uses HPACK which is used to split data from header.it compresses the header. 
The server sends all the other files like CSS & JS without the request of the client using the PUSH frame.

HTTP/1.1                                               
1.It works on the textual format.	  
2.There is head of line blocking that blocks 
all the requests behind it until it doesn’t
get its all resources.	                                                     
3.It uses requests resource Inlining for use 
getting multiple pages.
4.It compresses data by itself.

HTTP/2
1.it works on binary protocol.
2.it allows multiplexing so one TCP connection
is required for multiple requests
3.it uses push frame by server that
collects all multiple pages
4.it uses HPACK for data compression.

     
OBJECTS AND ITS INTERNAL REPRESENTATION IN JAVASCRIPT

Objects, in JavaScript, is it’s most important data-type and forms the building blocks for modern JavaScript. 
These objects are quite different from JavaScript’s primitive data-types(Number, String, Boolean, null, undefined and symbol) 
in the sense that while these primitive data-types all store a single value each (depending on their types).

Objects are more complex and each object may contain any combination of these primitive data-types 
as well as reference data-types. An object, is a reference data type. Variables that are assigned a reference 
value are given a reference or a pointer to that value. That reference or pointer points to the 
location in memory where the object is stored. The variables don’t actually store the value.

objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, 
in the form of “key: value” pairs. These keys can be variables or functions and are called properties 
and methods, respectively, in the context of an object.
