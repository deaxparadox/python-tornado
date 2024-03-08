# Long Polling

Long polling is itself not a true push; long polling is a variation of the traditional polling technique, but it allows emulating a push mechanism under circumstances where a real push is not possible, such as sites with security policies that require rejection of incoming HTTP requests.


With long polling, the client requests to get more information from the server exactly as in normal polling, but with the expectation that the server may not respond immediately. If the server has no new information for the client when the poll is received, then instead of sending an empty response, the server holds the request open and waits for response information to become available. Once it does have new information, the server immediately sends an HTTP response to the client, completing the open HTTP request. Upon receipt of the server response, the client often immediately issues another server request. In this way the usual response latency (the time between when the information first becomes available and the next client request) otherwise associated with polling clients is eliminated

For example, [BOSH](https://en.wikipedia.org/wiki/BOSH_(protocol)) is a popular, long-lived HTTP technique used as a long-polling alternative to a continues TCP connection when such as connection is difficult or impossible to employ directly.