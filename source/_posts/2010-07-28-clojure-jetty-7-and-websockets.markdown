---
layout: post
title: "Clojure, Jetty 7 and WebSockets"
date: 2010-07-28 12:00
comments: true
external-url:
categories: [clojure, jetty, websockets]
alias: "index.php/2010/07/28/clojure-jetty-7-and-websockets/"
---
I found this [gist][1] by Chris McDevitt&nbsp;which is a simple chat server and browser client that uses Jetty 7, Clojure and WebSockets.

I turned out to be quite a hassle to get it running so I thought I would document it here so others might save some time.

I have create a [project][2] on github that includes all the dependencies. I run it in Emacs using swank-clojure-project. The two last forms start the two servers – one is the websocket chat server, the other just serves the index.html file (this is necessary for the web_socket.js&nbsp; to work). I have only been able to make this work in browsers with native websocket support (Chrome and Safari). If anybody can figure out what goes wrong in the other browsers (e.g. Firefox) let me know, and I will update.

[1]: http://gist.github.com/281490
[2]: http://github.com/maacl/websocket-test
  
