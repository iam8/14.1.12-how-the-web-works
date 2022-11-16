
# 14.1.12-how-the-web-works

Contains my code and written responses for the 14.1 subunit exercise.

Note: Some exercise questions do not require a response of any kind (e.g. Part Four), so I have simply indicated that I completed the task it asked me to do.

## Part One: Solidify Terminology

- HTTP (Hypertext Transfer Protocol) is a web protocol that lays out a set of rules machines must use to communicate with each other over the web.
- A URL (Uniform Resource Locator) is a string of text denoting a path (address) to a resource on the web. It contains: protocol, hostname, port, resource, and query (in that order).
- DNS (Domain Name System) translates a given hostname (such as www.site.com) into an IP address, or vice versa (reverse lookup).
- A query string is a string of key-value pairs (optionally) appended to a URL. It contains extra arguments to send in a request over the web.
- Two HTTP verbs are GET and POST (most commonly used). The difference lies in the intention of the request - a GET request intends to retrieve some data or resource without altering the server data while a POST request intends to modify the server data.
- An HTTP request is sent by a client to a server over the web (via the HTTP protocol), in which the client specifies something of the server. For example, the client might request some data or the content of a resource, or the client might want to add new data to the server.
- An HTTP response is the requested resource or data sent back to the client by the server (via the HTTP protocol), if found. A response always contains a status code, indicating if the operation was successful.
- An HTTP header contains metadata relating to the request or response. Examples include: accept-language, accept-encoding, cookie (request); content-type, content-length, server, last-modified (response).
- When typing in a web address (such as http://somesite.com/some/page.html) into a browser, first the DNS attempts to resolve the hostname into an IP address; if successful, the machine with that IP address is connected to, and a GET request for the requested resource (some/page.html) is issued to that machine. The machine will then send back a response containing a status code and the requested resource (if found). The browser then sends out additional requests if the resource requires it (CSS, JS scripts, etc.) before assembling and displaying the final result.

## Part Two: Practice Tools

- curl -H "Accept: text/plain" https://icanhazdadjoke.com/search?term=pirate
- dig icanhazdadjoke.com (results in 2 IP addresses)
- Completed. Sample webpage is called sample_webpage.html, and can be reached via localhost:8000 or 127.0.0.1:8000 in the browser.

## Part Three: Explore Dev Tools

- The request and response headers can be viewed under the "Network" upper tab in Chrome DevTools, then clicking on the name of the request we just made, and then under the tab "Headers".
- After changing the form type to POST, refreshing, and resubmitting, the fields are not visible as a query string in the URL anymore.
- The form data can be viewed under the "Network" upper tab in Chrome DevTools, then clicking on the name of the request we just made, and then under the tab "Payload".

## Part Four: Explore the URL API

- Completed in Chrome console. Tried code examples from main URL API page and from page on URL() constructor.
