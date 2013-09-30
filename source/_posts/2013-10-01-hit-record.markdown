---
layout: post
title: "Hit Record!"
date: 2010-09-30 16:29
comments: true
external-url:
categories: [java, jmc, java_flight_recorder]
---

Richard Baeckman just did an excellent presentation on [Java Flight Recorder](http://www.oracle.com/technetwork/java/javaseproducts/mission-control/java-mission-control-1998576.html) at [goto Aarhus 2013](http://gotocon.com/aarhus-2013/). Java Flight Recorder is an - enhanced - port of JRockit Flight Recorder to the Oracle(Sun) JVM. It ships with  Java SE Development Kit 7u40 and includes a very nifty GUI called Java Mission Control that provides an excellent overvie of all the data collected in your recordings. I was very interested in seeing how useful JFR is when running Clojure code. Fortunately installation is very easy. After installing [Java Platform (JDK) 7u40](http://www.oracle.com/technetwork/java/javase/downloads/index.html) I just added the following options to my project.clj file.

` :jvm-opts ["-XX:+UnlockCommercialFeatures" "-XX:+FlightRecorder"] `

On OS X you have to start the JMC from a terminal invoking the binary located at:

`/Library/Java/JavaVirtualMachines/jdk1.7.0_40.jdk/Contents/Home/bin/jmc`

This brings up the JMC GUI. If you start your Clojure app (in my case Rich's ants.clj), your jvm(s) should be visible under the JVM Browser tab. From here you can start a recording by double-clicking the relevant JVM, right-clicking the Flight Recorder entry and choosing "Start Flight Recording...". I have inlcuded a screenshot below of a 1 minute recording of ants.clj. As you can tell JFR collects an immense amount of information but the overhead is minimal, approx 3% according to Richard.

![Java Mission Control](/images/posts/jmc.png "Java Mission Control Screenshot")

Please do note that the Java Flight Recorder and JMC are both Commercial Features, which I have written about previously [here](http://www.spyfoos.com/blog/2011/07/28/oracle-java-7-and-commercial-features/). This means that neither JFR and JMC may not be used for production purposes without a separate license from Oracle for such use. There is currently no public information regarding prices and other conditions available from Oracle.
