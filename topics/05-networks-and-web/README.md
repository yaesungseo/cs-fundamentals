# Networks and the Web
## Core idea
Networking connects programs running on different machines. Different protocols solve different parts of that communication problem.

## Follow a web request
1. A client resolves a hostname through DNS when it does not already have a usable cached answer.
2. It establishes the transport and security context required by the selected protocol.
3. It sends an HTTP request.
4. A server returns an HTTP response containing a status, headers, and possibly a body.

This is a simplified outline; connection reuse, caches, proxies, and protocol versions change the details.

## Essential vocabulary
- **IP:** addressing and packet delivery across networks.
- **Port:** helps identify a transport endpoint on a host.
- **TCP:** provides a reliable, ordered byte stream.
- **UDP:** sends datagrams without built-in guarantees of delivery or ordering.
- **DNS:** associates names with records, including address records.
- **HTTP:** defines application-level request and response semantics.
- **HTTPS:** HTTP protected using TLS. It protects transport confidentiality and integrity; it does not prove that a site's content is trustworthy.

HTTP/1.1 and HTTP/2 commonly use TCP. HTTP/3 uses QUIC over UDP. An application built on UDP can add reliability itself.

## Example
A successful TCP connection does not imply a successful application operation. An HTTP server may still return an error status.

## Try it
Explain the difference between “the hostname cannot be resolved,” “the connection failed,” and “the server returned 404.”

## Expand next
URLs; subnetting; sockets; HTTP methods and status codes; caching; cookies; TLS; proxies and load balancing.

[Back to index](../../README.md)
