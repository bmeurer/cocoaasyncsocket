## About

This is my fork of the [CocoaAsyncSocket](http://code.google.com/p/cocoaasyncsocket/) project.


## CocoaAsyncSocket

[CocoaAsyncSocket](http://code.google.com/p/cocoaasyncsocket/) supports TCP and UDP. The AsyncSocket class is for TCP, and the AsyncUdpSocket class is for UDP. Each class is described below.

**AsyncSocket** is a TCP/IP socket networking library that wraps `CFSocket` and `CFStream`. It offers asynchronous operation, and a native cocoa class complete with delegate support. Here are the key features:

- Queued non-blocking reads and writes, with optional timeouts. You tell it what to read or write, and it will call you when it's done.
- Automatic socket acceptance. If you tell it to accept connections, it will call you with new instances of itself for each connection. You can, of course, disconnect them immediately.
- Delegate support. Errors, connections, accepts, read completions, write completions, progress, and disconnections all result in a call to your delegate method.
- Run-loop based, not thread based. Although you can use it on main or worker threads, you don't have to. It calls the delegate methods asynchronously using NSRunLoop. The delegate methods include a socket parameter, allowing you to distinguish between many instances.
- Self-contained in one class. You don't need to muck around with streams or sockets. The class handles all of that.
- Support for TCP streams over IPv4 and IPv6.

The library is public domain, originally written by Dustin Voss. Now available in a public setting to allow and encourage its continued support.

**AsyncUdpSocket** is a UDP/IP socket networking library that wraps `CFSocket`. It works almost exactly like the TCP version, but is designed specifically for UDP. This includes queued non-blocking send/receive operations, full delegate support, run-loop based, self-contained class, and support for IPv4 and IPv6.


## License

CocoaAsyncSocket is [public domain](http://en.wikipedia.org/wiki/Public_domain).

