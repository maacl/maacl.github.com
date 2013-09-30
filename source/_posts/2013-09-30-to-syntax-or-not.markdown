---
layout: post
title: "To syntax or not"
date: 2010-09-30 11:00
comments: true
external-url:
categories: [syntax, javascript, douglas_crockford]
published: false
---
###Syntax

> In linguistics, syntax (from Ancient Greek σύνταξις "arrangement" from σύν syn, "together", and τάξις táxis, "an ordering") is "the study of the principles and processes by which sentences are constructed in particular languages".

Douglas Crockford just gave an interesting talk on programming language and how we are in love with the needlessly complicated syntax used in most languages. There was a lot of interesting from past and current programming languages, including some poor choices made by some otherwise very skillful language designers like Ken Thompson.

Douglas then proceeded to demonstrate how language parsing can be made much easier than it is usually assumed to be, using an approach called Top Down Operator Precedence. This approach was first presented in 1973 by Vaughan Pratt in his [paper](http://mauke.hopto.org/stuff/papers/p41-pratt.pdf) "Top Down Operator Precedence". Douglas has implemented a simplified Javascript parser using this approach which can 

 `var expression = function (rbp) {
        var left;
        var t = token;
        advance();
        left = t.nud();
        while (rbp < token.lbp) {
            t = token;
            advance();
            left = t.led(left);
        }
        return left;
    };`

I don't think it was entirely clear from the talk but I think Douglas' point in presenting this very simple approach to language parsing was to encourage more experimentation in language design. I 

While the TDOP certainly appears to be a very elegant approach to parsing I am not immediately convinced that it is much simpler in actual usage than for instance Clojure's [instaparse](https://github.com/Engelberg/instaparse). 
