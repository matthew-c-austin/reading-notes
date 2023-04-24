# Read: Class 09

## Reflections

This reading assignment is a refresher on the HTTP cycle, as well as some more in depth information than what we've covered at Code Fellows so far. The 5 steps to the lifecycle, the 4-way handshake for a TCP connection, and one method to do HTTP requests in Java.

## Readings

[Review: High-level HTTP](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

1. What are the five steps in the HTTP Request Lifecycle?

   1. **DNS Lookup**:  
   The client initiates the process by resolving the domain name of the server into an IP address. This is done using the Domain Name System (DNS) to find the server's IP address that matches the domain name provided in the URL.

   2. **TCP Connection**:  
   Once the IP address is resolved, the client establishes a Transmission Control Protocol (TCP) connection with the server. TCP is a reliable, connection-oriented protocol that ensures that data packets are transmitted correctly and in order.

   3. **Send HTTP Request**:  
   After the TCP connection is established, the client sends an HTTP request to the server. This request consists of an HTTP method (e.g., GET, POST, PUT, DELETE), a URL path, and any additional headers or data (e.g., cookies, authentication tokens) needed for the server to process the request.

   4. **Server Processes Request and Sends Response**:  
   The server receives the HTTP request, processes it, and generates an HTTP response. The response consists of a status code (e.g., 200 OK, 404 Not Found), headers (e.g., content-type, cache-control), and the actual content (e.g., HTML, JSON, images).

   5. **Close TCP Connection**:  
   Once the response is sent back to the client, the TCP connection is typically closed, unless the "keep-alive" feature is used, which allows multiple requests and responses to be sent over a single connection. The client processes the response, rendering the content or performing additional actions based on the status code and headers.

2. What are the two things the client needs before it can make an HTTP Request?

    An IP address and a TCP connection

3. Explain the four way handshake and what it does.

    The four-way handshake is a process that ensures a reliable, connection-oriented communication between two devices using TCP. It consists of four messages that allow the devices to establish, use, and gracefully terminate the connection. Here's an overview of the four-way handshake:

    1. SYN: The client initiates the connection by sending a segment with the SYN (Synchronize Sequence Numbers) flag set. This message informs the server that the client wants to establish a connection and provides an initial sequence number.

    2. SYN-ACK: In response to the client's SYN, the server sends a segment with the SYN and ACK (Acknowledgment) flags set. The SYN part indicates that the server is willing to establish a connection, while the ACK part acknowledges the client's SYN. The server also provides its initial sequence number.

    At this point, the connection is considered established, and both devices can start exchanging data using the reliable, connection-oriented features provided by TCP.

    3. FIN: When one of the devices (e.g., the client) wants to close the connection, it sends a segment with the FIN (Finish) flag set. This message informs the other device (e.g., the server) that the sender has finished sending data and wants to terminate the connection.

    4. FIN-ACK: In response to the FIN, the other device (e.g., the server) sends a segment with the ACK flag set, acknowledging the receipt of the FIN message. The device may also send its own FIN message in the same segment (or separately) to indicate that it has also finished sending data.

    Once the FIN and FIN-ACK messages are exchanged, the connection is considered closed, and both devices can release the resources associated with the connection.

[Java HTTP Request example](https://www.baeldung.com/java-http-request)

1. True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.

    False, this is an option that you can enable or disable by using the `setInstanceFollowRedirects()` method with a `true` or `false` parameter.

2. Which built-in Java class can be used to perform an HTTP request?

    `HttpUrlConnection`, however with JDK 11, a new API is introduced that is meant as a replacement, the `HttpClient` API.

3. What HTTP status codes represent a successful response? A redirect? A client error?

    `2XX`, `3XX`, `4XX`

## Things I want to know more about

1. Are these the types of questions that would come up in an interview setting? Like "explain the 4-way handshake for an HTTP request."
2. Are we planning learning the `HttpClient` API in this course? The `HttpUrlConnection` method seems extremely verbose.
