# Introduction

Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed. By using non-blocking network I/O, Tornado can scale to tens of thousands of open connections, making it ideal for long polling, WebSockets, and other applications that require a long-lived connection to each user.

Tornado can be rougly divided into three major components:

- A web framework (including **`RequestHandler`** which is subclassed to create web applications, and various supporting classes).
- Client- and server-side implementions of HTTP (**`HTTPServer`** and **`AsyncHTTPClient`**).
- An asynchronous