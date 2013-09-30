---
layout: post
title: "Oracle vs Google - Implementing the JVM Specification"
date: 2010-08-24 12:00
comments: true
external-url:
categories: [google, oracle, jvm, copyright, specification, android, dalvik, java, patents]
alias: "index.php/2010/08/24/oracle-vs-google-implementing-the-java-specification/"
---
A lot has already been written on the Oracle vs. Google Android [case][1]. [Some][2] of it is brilliant. [Some][3] is illuminating, [some][4] less so. Since the complaint is devoid of any details as to how Android infringes upon the patents listed in the complaint, I will focus on the alleged copyright infringement. Here too Oracle is not specific but it is clear that the infringement is alleged at least in part on the basis of unlicensed use of specification(s) in which Oracle holds copyright(cf. Count VIII section 38 of the complaint) .

For context Oracle in the complaint defines Android as:

The Android operating-system software “stack” consists of Java applications running on a Java-based object-oriented application framework, and core libraries running on a “Dalvik” virtual machine (VM) that features just-in-time (JIT) compilation.

One aspect that appears to confuse matters is what [Dalvik][5] is. Dalvik is VM but *not* a Java VM. Dalvik executes .dex files which are created from .class files produced by a Java compiler. The .dex files are created by a tool called “dx”. As such Dalvik does not implement the Java Language Specification. The “dx” tool does however appear to implement part of the Java [Virtual Machine Specification][6], namely [the part][7] that specifies the .class file format. As the “dx” tool does not comply with the conditions of SUN’s [license grant][8] the question is then: Does Google need a copyright license from SUN to implement the “dx” tool?

From a European perspective the recent SAS vs. World Programming(WPL) case sheds some very interesting light on this issue. The case a addresses the application of copyright to programming languages, interfaces and functionality. While the judge submits all of the questions to the ECJ for a preliminary ruling, he clearly thinks, on the strength English precedents(specifically the Navitaire [case][9]) that neither programming languages, interfaces or functionality is protectable by copyright. If the ECJ concurs with the judges&nbsp;opinion it is hard to see why Google would need a license to implement the .class file format as part of their “dx” tool.

Would the analysis under US copyright law be the same?

   [1]: http:/www.scribd.com/doc/35811761/Oracle-s-complaint-against-Google-for-Java-patent-infringement
   [2]: http://blog.headius.com/2010/08/my-thoughts-on-oracle-v-google.html
   [3]: http://tirania.org/blog/archive/2010/Aug-13.html
   [4]: http://fosspatents.blogspot.com/2010/08/oracle-vs-google-licensing-issues.html
   [5]: http://en.wikipedia.org/wiki/Dalvik_(software)
   [6]: http://java.sun.com/docs/books/jvms/second_edition/html/VMSpecTOC.doc.html
   [7]: http://java.sun.com/docs/books/jvms/second_edition/html/ClassFile.doc.html
   [8]: http://java.sun.com/docs/books/jvms/second_edition/html/Copyright.doc.html
   [9]: http://www.bailii.org/ew/cases/EWHC/Ch/2004/1725.html

  
