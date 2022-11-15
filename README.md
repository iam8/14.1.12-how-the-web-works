
# 14.1.12-how-the-web-works

Contains my code and written responses for the 14.1 subunit exercise.

Note: Some exercise questions do not require a response of any kind (e.g. Part Four), so I have simply indicated that I completed the task it asked me to do.

## Part One: Solidify Terminology

- HTTP (Hypertext Transfer Protocol) is a web protocol that lays out a set of rules machines must use to communicate with each other over the web.
- A URL is a string of text denoting a path to a resource on the web. It contains: protocol, hostname, port, resource, and query (in that order).
- DNS (Domain Name System) translates a given hostname (such as www.site.com) into an IP address, or vice versa (reverse lookup).
- A query string is (optionally) appended to a URL. It contains extra arguments to send in a request over the web.
- Two HTTP verbs are GET and POST (most commonly used). The difference lies in the intention of the request - a GET request intends to retrieve some data or resource without altering the server data while a POST request intends to modify the server data.
- An HTTP request is sent by a client to a server over the web (via the HTTP protocol), in which the client specifies something of the server. For example, the client might request some data or the content of a resource, or the client might want to add new data to the server.
- An HTTP response is the requested resource or data sent back to the client by the server, if found. A response always contains a status code, indicating if the operation was successful.
- An HTTP header contains metadata relating to the request or response. Examples include: accept-language, accept-encoding, cookie (request); content-type, content-length, server, last-modified (response).
- When typing in a web address (such as http://somesite.com/some/page.html) into a browser, first the DNS attempts to resolve the hostname into an IP address; if successful, the machine with that IP address is connected to, and a GET request for the requested resource (some/page.html) is issued to that machine. The machine will then send back a response containing a status code and the requested resource (if found).

## Part Two: Practice Tools

- curl -H "Accept: text/plain" https://icanhazdadjoke.com/search?term=pirate
- dig icanhazdadjoke.com (results in 2 IP addresses)
- Completed

## Part Three: Explore Dev Tools

## Part Four: Explore the URL API