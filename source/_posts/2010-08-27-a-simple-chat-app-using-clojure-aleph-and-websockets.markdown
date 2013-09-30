---
layout: post
title: "A Simple Chat App Using Aleph, Websockets and Clojure"
date: 2010-08-27 12:00
comments: true
external-url:
categories: [clojure, netty, aleph, websockets]
alias: "index.php/2010/08/27/a-simple-chat-app-using-aleph-websockets-and-clojure/"
---
I have implemented a small example shoving how to use the websocket support in [Aleph][1], asynchronous webframework for [Clojure][2] built on [Netty][3].

The example is tested with Chrome and Firefox on Ubuntu. It should work in all modern browsers as it relies on [web-socket-js][4] for websocket emulation in browsers that do not have native support. Please note the updated Usage instructions. The socket-policy-server necessary for Flash websocket emulation has to listen on port 843 (at least that is the first place Flash asks for the policy file) so the server has to be run using sudo.

If you are interested the example is at hosted on [github][5], along with usage instructions.

   [1]: http://github.com/ztellman/aleph
   [2]: http://clojure.org/
   [3]: http://www.jboss.org/netty
   [4]: http://github.com/gimite/web-socket-js/
   [5]: http://github.com/maacl/aleph-ws-test

  
