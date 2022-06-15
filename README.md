1. Write a blog on difference between http / 1.1 vs http /2  ?

HTTP2 is much faster and more reliable than HTTP1. HTTP1 loads a single request for every TCP connection, while HTTP2 avoids network delay by using multiplexing. HTTP is a network delay sensitive protocol in the sense that if there is less network delay, then the page loads faster.


HTTP/2 improved on HTTP/1.1 in a number of ways that allowed for speedier content delivery and improved user experience.




                            HTTP / 1.1                                                                HTTP / 2
the usest works on the textual format.	                                  It works on the binary protocol.
There is head of line blocking that blocks all the requests behind        It allows multiplexing so one TCP connection is required for multiple requests.
it until it doesn’t get its all resources.	
It uses requests resource Inlining for use getting multiple pages	        It uses PUSH frame by server that collects all multiple pages
It compresses data by itself.	                                            It uses HPACK for data compression.


MAIN ADVANTAGE OF HTTP /2 OVER HTTP / 1.1 
The primary advantage of HTTP/2 is its improved speed over HTTP/1.1. This is achieved thanks to a combination of elements: HTTP/2 is binary, instead of textual meaning it is more compact, travels faster 'on the wire' and is less susceptible to errors. HTTP/2 is fully multiplexed.



2. Write a blog about objects and its internal representation in Javascript 

   

Objects and its internal representation in Javascript
Object:


In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.
Creating Objects in JavaScript:
    #By object literal
    #By creating instance of Object directly (using new keyword)


By object literal:
The syntax of creating object using object literal is given below:

Property and value is separated by colon(:).

Example:
Var person = {
fname:”xxx”,
lname=“yyy”,
Age:23
};


By creating instance of Object directly (using new keyword):
The syntax of creating object directly is given below:

Var objectname=new Object();


Here, new keyword is used to create object.
Example:

Var emp=new Object();
Emp.id=101;
Emp.name=“xxx”;
Emp.salary=50000;


Accessing JavaScript Objects:
The syntax for accessing the property of an object is:


objectName.property

or

objectName[“property”]


Accessing ‘fname’ from example 1 using dot operator,
     
    Person.fname


Accessing ‘name’ form example 2 using [],
     

     emp[“name”]




