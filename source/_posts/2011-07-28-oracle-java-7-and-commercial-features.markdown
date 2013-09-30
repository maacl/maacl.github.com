---
layout: post
title: "Oracle Java 7 and 'Commercial Features'"
date: 2011-07-28 12:00
comments: true
external-url:
categories: [copyright, evil, oracle, jvm, license, sla]
alias: "index.php/2011/07/28/oracle-java-7-and-commercial-features/"
---
Oracle has just announced the general availability of Java 7 SE including Java SE Advanced and Java SE Suite.

Being a software license nerd I of course skimmed the [Java SE License Agreement ][1](full title “Oracle Binary Code License Agreement for the Java SE Platform Products”).

The license contains some interesting wording regarding “Commercial Features” in section 1, 2 and SUPPLEMENTAL LICENSE TERMS section A and G. The “Commercial Features” are defined in [this][2] document (PDF version with better layout [here][3]). Please note that the specification of “Commercial Features” is not part of the license as such and therefor subject to change at Oracle’s discretion.

![jvm_commercial_features_table](/images/posts/jvm_commercial_features_table.png "JVM Commercial Features Table")

It turns out the “Commercial Features” are subject to rather draconian restrictions (SUPPLEMENTAL LICENSE TERMS section A):

> COMMERCIAL FEATURES You may not use the Commercial Features for running Programs, Java applets or applications in your internal business operations or for any commercial or production&nbsp; purpose, or for any purpose other than as set forth in Sections B, C, D and E of these Supplemental Terms.&nbsp; If You want to use the Commercial Features for any purpose other than as permitted in this Agreement, You must obtain a separate license from Oracle.

As you can tell any meaningful business use of the “Commercial Features” are subject to a separate license.

So does the regular Java 7 SE download contain any of these “Commercial Features”? It does not look like it and the Java Se Advance and Java SE Suite packages doesn’t either, because they do not exist. From below two sections that appear at end of [this ][2]document, it is clear that the Java SE Advanced and Java SE Suite “products” are a combination of the Java 7 SE and a number of separate packages.

> ## Installation of Java SE Product Editions
>
> Oracle does not provide installation programs that correspond directly to Java SE, Oracle Java SE Advanced and Oracle Java SE Suite. Depending on the features licensed, one or more of the following individual packages must be downloaded:
>
> JRE&nbsp;JDK
>
> JRockit JDK
>
> JRockit Mission Control
>
> Java for Business JRE
>
> Java for Business JDK
>
> ### Licensing Considerations and Restricted-Use Licensing
>
> Some of the packages described in Installation of Java SE Product Editions install commercial features that are restricted to Oracle Java SE Advanced or Oracle Java SE Suite. For example, the JRockit JDK comes with a deterministic garbage collector that requires a Oracle Java SE Suite license.

If you download (which you can do for instance [here][4] and [here][5]) and use these extra packages for the purposes outlined above (any meaning full business use) in combination with Java 7 SE you are subject to a separate (ostensibly payable) license.

The only mention I can find of this change from Oracle is [this][6] blog post with the clearly misleading title “JRockit is Now Free (and Other Java License Updates)”, as this does not apply to the JRockit “Commercial Features” listed above.

You should make sure that your developers, ops people and relevant vendors of such service knows this, or you could end up breaching your license and owing Oracle a lot of money.

   [1]: http://www.oracle.com/technetwork/java/javase/terms/license/index.html
   [2]: http://www.oracle.com/technetwork/java/javase/terms/products/index.html
   [3]: http://www.oracle.com/technetwork/java/javase/documentation/java-se-product-editions-397069.pdf
   [4]: http://www.oracle.com/technetwork/java/javase/downloads/jrefb-5u30-download-401429.html
   [5]: http://www.oracle.com/technetwork/middleware/jrockit/downloads/index.html
   [6]: http://blogs.oracle.com/henrik/entry/jrockit_is_now_free_and
  
