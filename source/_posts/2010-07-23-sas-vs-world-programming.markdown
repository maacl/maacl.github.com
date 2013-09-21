---
layout: post
title: "SAS vs. World Programming"
date: 2010-07-23 12:00
comments: true
external-url:
categories: [copyright, sas, world_programming, software]
alias: "index.php/2010/07/23/sas-vs-world-programming/"
---

UPDATE: I did a follow-up post on the SAS Press Release [here][1]

So the [decision][2] in “SAS Institute Inc v World Programming Ltd” has been published and it is in favor of WPL on all counts, except that the judge finds that WPL – against it’s own policy – copied certain language from SAS’ manuals into its own manuals.

Key questions pertaining to almost all the other claims will be submitted to the ECJ for confirmation of the judges interpretation of the law(specifically Articles 1(2) and 5(3) of the [Software Directive][3] and Article 2(a) of the [Information Society Directive][4]) (see below).

If everything holds up this is potentially a huge win for competition in the software industry.The decision means that can re-implement the functionality of other software and reference that software and its documentation in the process, as long as you do not copy any source code or documentation. The judge (who appears to be quite technically savvy) analyses in detail how the SAS language is constructed. SAS appears to argue that the PROCS steps in the SAS Language is not a programming language, but in fact a computer program in itself. The SAS expert Dr. Ivey states the following on the matter:

&gt; the SAS Language was a domain specific computer language with many of the attributes of a command language, rather than a programming language

It is not clear to me exactly what SAS was hoping to achieve with this line of reasoning ([perhaps they were trying to escape a suspected non-copyrightability of programming languages][5]) but whatever it was it did not work as the judge slightly sarcastically [finds][6] that:

&gt; In my judgment the SAS Language is a programming language. I am comforted by the fact that this assessment coincides not only with SAS Institute’s own assessment in paragraph 6 of its Particulars of Claim and in its literature, but also with that of the anonymous author of the entry for “SAS language” in Wikipedia (as last modified on 25 April 2010), which states:
&gt;
&gt; “… SAS can be considered a general programming language, though it serves largely as a database programming language and a language with a wide variety of specialized analytic and graphic procedures.”

The judge also analyses whether the _functionality _of a computer program (not the source code) is itself protectable by copyright and [finds][7] that:

&gt; Accordingly, I consider that the functionality of a computer program falls on the wrong side of the line drawn by Article 1(2) of the Software Directive, Article 9(2) of TRIPS and Article 2 of the WIPO Copyright Treaty.

So the functionality of a computer program is not protectable, which is not too surprising, but as the question in the judges opinion is not _[acte clair_][8] it is submitted together with 5 other questions ([para 332][9] i, ii, iii, v, vi and viii)) to the ECJ for guidance. Among these is also the question of whether a programming language as such is protectable by copyright. The judge finds that this is probably not the case, but appears less certain on this question than the others.

It will be really interesting to see if this will result alternative vendors deciding to challenge other dominant software products, by producing compatible solutions that release the customers from lock-in and introduce effective competition.

   [1]: http://www.spyfoos.com/index.php/2010/07/29/sas-vs-world-programming-sas-version/
   [2]: http://www.bailii.org/ew/cases/EWHC/Ch/2010/1829.html
   [3]: http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:31991L0250:EN:HTML
   [4]: http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:32001L0029:EN:HTML
   [5]: http://news.ycombinator.com/item?id=1545404
   [6]: http://www.bailii.org/ew/cases/EWHC/Ch/2010/1829.html#para56
   [7]: http://www.bailii.org/ew/cases/EWHC/Ch/2010/1829.html#para236
   [8]: http://www.translegal.com/legal-english-dictionary/acte-clair
   [9]: http:/www.bailii.org/ew/cases/EWHC/Ch/2010/1829.html#para332
