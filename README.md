# EWebSocket
This library is a fork of the [websocket module](https://github.com/vlang/v/tree/master/vlib/net/websocket) of the V standard library.
<br>It uses [TLSe](https://github.com/eduardsui/tlse) instead of OpenSSL to implement Transport Layer Security.

## Advantages of TLSe over OpenSSL
* Smaller executables
* Easier deployment
* More permissive licenses (public domain, BSD or MIT)

## Why is all the code in another submodule?
The actual websocket module lives inside the submodule "websocket" of this "ewebsocket" module.
<br>This is for easier conversion between the original websocket module and this fork.

## Dependencies
* [tlse](https://github.com/Wertzui123/TLSe) (a TLSe wrapper for V)
* [ehttp](https://github.com/Wertzui123/ehttp) (a custom version of the `net.http` module that uses TLSe instead of OpenSSL)