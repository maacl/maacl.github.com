---
layout: post
title: "Om, Clojure/ClojureScript and Event Sourcing"
date: 2014-09-09 22:00
comments: true
external-url:
categories: [om, clojurescript, clojure, event_sourcing, david_nolen, greg_young, gotocph, react.js]
---
[goto CPH](http://gotocon.com/cph-2014/) is closing in rapidly.

As mentioned previously I am especially looking forward to  [David Nolen's](http://gotocon.com/cph-2014/speaker/David+Nolen) talk [Putting the Dream Machine to Work](http://gotocon.com/cph-2014/presentation/Immutability:%20Putting%20The%20Dream%20Machine%20To%20Work).

[Om](https://github.com/swannodette/om) is getting a lot of coverage and even if it is still very new, it is seeing some heavy duty prodcution usage, for instance at [Prismatic](http://www.getprismatic.com/). But Prismatic has gone even further that just using Om and released [om-tools](https://github.com/Prismatic/om-tools), which makes it even more straight forward to use Om. I especially like how it smoothes over some of the slightly ugly Javascript interop that Om requires out of the box.

Another talk I am looking very much forward to is [Greg Young's talk on Event Sourcing](http://gotocon.com/cph-2014/presentation/Event-sourcing). Event Sourcing is a very interesting [pattern](http://martinfowler.com/eaaDev/EventSourcing.html) which has a very natural fit to many common business scenarios, and I am looking forward to Greg Young giving us some examples of that. The benefits of the event sourcing pattern appears to me to overlap somewhat with the benefits of the Clojure based database [Datomic](http://www.datomic.com/) which also emphazises the need for a solid model of time.

If you are interested in dabbling with Event Sourcing and have been inspired by David's talk on Om/ClojureScript you should check out the [JVM Soup post on Event Sourcing in Clojure](http://jvmsoup.com/2014/06/23/clojure-websockets-server-and-event-sourcing/). This post demonstrates how to use [core.async](https://github.com/clojure/core.async) Clojure/ClojureScripts CSP implentation, which David also recommends to do inter component communication when using Om, to do event sourcing in Clojure/ClojureScript.
