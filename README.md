# python-tornado

## Learn tornado

Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed. By using non-blocking network I/O, 

Tornado can scale to tens of thousands of open connections, making it ideal for [long polling](learn/101-long-polling.md), [WebSockets](learn/102-websocket.md), and other applications that require a long-lived connection to each user.


----------


Code:

- [Hello to Tornado](code/101_hello_world.py)


### Threads and WSGI

Tornado is different from most Python web frameworks. It is based on [WSGI](https://), and it is typically run with only one thread per process.


## User Guide

- [Introduction](guide/101_introduction.md)