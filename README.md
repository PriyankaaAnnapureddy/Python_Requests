## Objectives

After completing this lab you will be able to:

* Understand HTTP    
* Handle HTTP Requests


Overview of HTTP 
When you, the client, use a web page your browser sends an HTTP request to the server where the page is hosted. The server tries to find the desired resource by default "index.html". If your request is successful, the server will send the object to the client in an HTTP response. This includes information like the type of the resource, the length of the resource, and other information.

The figure below represents the process. The circle on the left represents the client, the circle on the right represents the Web server. The table under the Web server represents a list of resources stored in the web server. In this case an HTML file, png image, and txt file .

The HTTP protocol allows you to send and receive information through the web including webpages, images, and other web resources. In this lab, we will provide an overview of the Requests library for interacting with the HTTP protocol.


Uniform Resource Locator: URL
Uniform resource locator (URL) is the most popular way to find resources on the web. We can break the URL into three parts.

scheme this is this protocol, for this lab it will always be http://
Internet address or Base URL this will be used to find the location here are some examples: www.ibm.com and  www.gitlab.com 
route location on the web server for example: /images/IDSNlogo.png
You may also hear the term Uniform Resource Identifier (URI), URL are actually a subset of URIs. Another popular term is endpoint, this is the URL of an operation provided by a Web server.

Request 
The process can be broken into the request and response process. The request using the get method is partially illustrated below. In the start line we have the GET method, this is an HTTP method. Also the location of the resource /index.html and the HTTP version. The Request header passes additional information with an HTTP request:


When an HTTP request is made, an HTTP method is sent, this tells the server what action to perform. A list of several HTTP methods is shown below. We will go over more examples later.


Response
The figure below represents the response; the response start line contains the version number HTTP/1.0, a status code (200) meaning success, followed by a descriptive phrase (OK). The response header contains useful information. Finally, we have the response body containing the requested file, an  HTML  document. It should be noted that some requests have headers.


Some status code examples are shown in the table below, the prefix indicates the class. These are shown in yellow, with actual status codes shown in white. Check out the following link for more descriptions.

