                
                Create a REST request to get started: https://www.googleapis.com/books/v1/volumes?q=turing

Request Header: 
	GET https: //www.googleapis.com/books/v1/volumes?q=turing HTTP/1.1
	Accept-Encoding: gzip, deflate
	Host: www.googleapis.com
	Connection: Keep-Alive
	User-Agent: Apache-HttpClient/4.1.1(java 1.5)

Descriptions: 

1.	The client uses GET to send a request to server by HTTP protocol and server sends back a copy of the document required. "method" - the HTTP method for this request (e.g. "GET", "POST", "HEAD",  etc.,) "version" - the HTTP version of this request (e.g. "HTTP/1.1"). HTTP/1.1 is a pipelined protocol that sent by client to get a document q=turing.
2.	Accept-Encoding restricts the content-codings that are acceptable in the response such as gzip, deflate.
3.	Host request-header specifies the Internet host and port number of the resource being requested, as obtained from the original URI given by the user or referring resource. Its value must represent the naming authority of the origin server or gateway given by the original URL. So, its value is www.googleapis.com.
4.	Connection header field allows the sender to specify options that are desired for that particular connection. Its value – keep alive means that connection is considered `connected' after the current request/response is complete.
5.	User agent request-header field contains information about the user agent originating the request. In this case, this is a client/server request. Server is Apache server and Http/Client is client side (using Java 1.5).



Response Header:

	HTTP/1.1 200 OK
	Expires: Fri, 06 Feb 2015 23:55:00 GMT
	Date: Fri, 06 Feb 2015 23:55:00 GMT
	Cache-Control: private, max-age=0, must-revalidate, no-transform
	ETag: "_rmWcTkH-s1QFjg9mc3XeI0FZSQ/R00mb_62rPUkmKxN5bUSZOaKe78"
	Vary: Origin
	Vary: X-Origin
	Content-Type: application/json; charset=UTF-8
	X-Content-Type-Options: nosniff
	X-Frame-Options: SAMEORIGIN
	X-XSS-Protection: 1; mode=block
	Content-Length: 28463
	Server: GSE
	Alternate-Protocol: 443:quic, p=0.02

Description: 

1.	“Status” - The HTTP response status code (e.g. "200" or "200 OK", meaning the request has succeeded)
2.	Expires entity-header field give the date/time after which the response is considered stale.
3.	Date header field represents the date and time at which the message was originated, having the same semantics as origin-date. The field value is an HTTP-date.
4.	Cache Control header field is used to specify directives that must be obeyed by all caching mechanisms along the request/response chain.
	Cache is controlled privately.
	max-age indicates that the client is willing to accept a response whose age is no greater than the specified time in seconds.
5.	ETag response-header field provides the current value of the entity tag for the requested variant
6.	Vary field value indicates the set of request-header fields that fully determines, while the response is fresh, whether a cache is permitted to use the response to reply to a subsequent request without revalidation.  Vary field value advises the user agent about the criteria that were used to select the representation.
7.	The same as above except for the value is X-Origin.
8.	Content-Type entity header field indicates the media type of the entity-body sent to the recipient or, in the case of the HEAD method, the media type that would have been sent had the request been a GET. Its value is application and json; charset is UTF-8.
9.	The only defined value, "nosniff", prevents Internet Explorer and Google Chrome from MIME-sniffing a response away from the declared content-type. This also applies to Google Chrome, when downloading extensions. This reduces exposure to drive-by download attacks and sites serving user uploaded content that, by clever naming, could be treated by MSIE as executable or dynamic HTML files. 
10.	 Provides Clickjacking protection. Values: deny - no rendering within a frame, SAMEORIGIN - no rendering if origin mismatches, allow-from: DOMAIN - allow rendering if framed by frame loaded from DOMAIN.
11.	 This header enables the Cross-site scripting (XSS) filter built into most recent web browsers. It's usually enabled by default anyway, so the role of this header is to re-enable the filter for this particular website if it was disabled by the user. This header is supported in IE 8+, and in Chrome (not sure which versions). The anti-XSS filter was added in Chrome 4. It’s unknown if that version honored this header.
12.	 Content-Length entity-header field indicates the size of the entity-body, in decimal number of OCTETs, sent to the recipient. Its value is 28463.
13.	 Server response-header field contains information about the software used by the origin server to handle the request. Its value is GSE.
14.	  Different protocols can be used. QUIC (Quick UDP Internet Connections)
	 

       


                      Create a SOAP endpoint by importing a WSDL as http://www.webservicex.net/geoipservice.asmx?wsdl

Request Header:

	POST http://www.webservicex.net/geoipservice.asmx HTTP/ 1.1
	Accept-Encoding: gzip, deflate
	Content-Type: text/xml; charset=UTF-8
	SOAPAction: http://www.webservicex.net/GetGeoIP
	Content-Length: 317
	Host: www.webservicex.net 
	Connection: Keep-Alive
	User-Agent: Apache-HttpClient/4.1.1(java 1.5)


Description:

1	The client uses POST to send a request to server by HTTP protocol and server appends the data to a specified item.
2	Accept-Encoding restricts the content-codings that are acceptable in the response such as gzip, deflate.
3	Content-Type entity header field indicates the media type of the entity-body sent to the recipient or, in the case of the HEAD method, the media type that would have been sent had the request been a POST. Its value is text and xml; charset is UTF-8.
4	SOAPAction indicates the action parameter carried in the application/soap+xml Content-Type header field. 
5	Content-Length entity-header field indicates the size of the entity-body, in decimal number of OCTETs, sent to the recipient. Its value is 317.
6	Host request-header specifies the Internet host and port number of the resource being requested, as obtained from the original URI given by the user or referring resource. Its value must represent the naming authority of the origin server or gateway given by the original URL. So, its value is www.webservicex.net.
7	Connection header field allows the sender to specify options that are desired for that particular connection. Its value – keep alive means that connection is considered `connected' after the current request/response is complete.
8	User agent request-header field contains information about the user agent originating the request. In this case, this is a client/server request. Server is Apache server and Http/Client is client side (using Java 1.5).



Response Headers:

	HTTP/1.1 200 OK
	Cache-Control: private, max-age=0
	Content-Type: text/xml; charset=utf-8
	Content-Encoding: gzip
	Vary: Accept-Encoding
	Server: Microsoft-IIS/7.0
	X-AspNet-Version: 4.0.30319
	X-Powered-By: ASP.NET
	Date: Fri, 06 Feb 2015 23:16:01 GMT
	Content-Length: 401


Description:

1	“Status” - The HTTP response status code (e.g. "200" or "200 OK", meaning the request has succeeded).
2	Cache Control header field is used to specify directives that must be obeyed by all caching mechanisms along the request/response chain.
	Cache is controlled privately.
	max-age indicates that the client is willing to accept a response whose age is no greater than the specified time in seconds
3	Content-Type entity header field indicates the media type of the entity-body sent to the recipient or, in the case of the HEAD method, the media type that would have been sent had the request been a POST. Its value is text and xml; charset is UTF-8.
4	Content-Encoding restricts the content-codings that are acceptable in the response such as gzip.
5	Vary field value indicates the set of request-header fields that fully determines, while the response is fresh, whether a cache is permitted to use the response to reply to a subsequent request without revalidation.  Vary field value advises the user agent about the criteria that were used to select the representation.
6	Server response-header field contains information about the software used by the origin server to handle the request. Its value is Microsoft-IIS/7.0 (Microsoft Internet Information Server, version 7.0).
7	X-AspNet-Version specifies the version of ASP.NET used. Its value is 4.0.30319.
8	X-Powered-By: ASP.NET - Indicates that the website is "powered by ASP.NET."
9	Date header field represents the date and time at which the message was originated, having the same semantics as origin-date. The field value is an HTTP-date.
10	Content-Length entity-header field indicates the size of the entity-body, in decimal number of OCTETs, sent to the recipient. Its value is 401.


