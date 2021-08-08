# https_desc

HTTP - HyperText Transfer Protocol for World wide web, developed by Tim Barnes-Lee and his team between 1989-91.

##Versions

HTTP v0.9 

Extremely simple: requests consist of a single line and start with the only possible method GET followed by the path to the resource

GET /myPage.html

#Limitations

Has no HTTP headers, only HTML page was sent over the internet.
No Status code or ERROR code, in case of any problem HTML page will be resent back

HTTP v1.0  

Versioning information is now sent within each request (HTTP/1.0 is appended to the GET line)
HTTP headers has been introduced, both for the requests and the responses, allowing metadata to be transmitted and making the protocol extremely flexible and extensible.
With the help of HTTP Headers other documents also can be sent other than HTML page using Content-Type header

HTTP v1.1 - Standardized  Protocol

A connection can be reused, saving the time to reopen it numerous times to display the resources embedded into the single original document retrieved.
Pipelining has been added, allowing to send a second request before the answer for the first one is fully transmitted, lowering the latency of the communication.
Chunked responses are now also supported.
Additional cache control mechanisms have been introduced.
Content negotiation, including language, encoding, or type, has been introduced, and allows a client and a server to agree on the most adequate content to exchange.
Thanks to the Host header, the ability to host different domains at the same IP address now allows server colocation.

HTTP v2 – A protocol for greater performance

Over the years, Web pages have become much more complex, even becoming applications in their own
In the first half of the 2010s, Google demonstrated an alternative way of exchanging data between client and server, by implementing an experimental protocol SPDY. This amassed interest from developers working on both browsers and servers. Defining an increase in responsiveness, and solving the problem of duplication of data transmitted, SPDY served as the foundations of the HTTP/2 protocol.

#Advantages
It is a binary protocol rather than text. It can no longer be read and created manually. Despite this hurdle, improved optimization techniques can now be implemented.
It is a multiplexed protocol. Parallel requests can be handled over the same connection, removing the order and blocking constraints of the HTTP/1.x protocol.
It compresses headers. As these are often similar among a set of requests, this removes duplication and overhead of data transmitted.
It allows a server to populate data in a client cache, in advance of it being required, through a mechanism called the server push.
