---
layout: post
title: "GOTO Aarhus 2013 - ClojureScript"
date: 2013-09-13 12:00
comments: true
external-url:
categories: [goto, clojurescript]
alias: "#/posts/20130913000000.markdown/"
---
I put together my first draft itenary for [GOTO Aarhus 2013](http://gotocon.com/aarhus-2013/). You can see it [here](http://gotocon.com/aarhus-2013/schedule/my-schedule.jsp#myschedlink1).

Fortunately the programme did not pose too many dilemma's for me to resolve, although choosing between "Obstacles And Patterns To Maximize Flow In IT Operations" and "Lambdas in Java: A peek under the hood" on Tuesday morning was a bit difficult.

I was especially pleased to see that [David Nolen](http://swannodette.github.io/) is giving a talk. David is fairly prolific in the [Clojure](http://clojure.org/) community. He is the driving force behind core.logic and a significant contributor to [ClojureScript](https://github.com/clojure/clojurescript). [Core.logic](https://github.com/clojure/core.logic) is a implementation of miniKaren and provides robust logic programming facilities in Clojure and [ClojureScript](https://github.com/clojure/clojurescript). As an example of how concise logic programming can be please see below Sudoku solver by David Nolen.

;; based on core.logic 0.8-alpha2 or core.logic master branch

    (ns sudoku
        (:refer-clojure :exclude [==])
            (:use clojure.core.logic))

    (defn get-square [rows x y]
        (for [x (range x (+ x 3))
              y (range y (+ y 3))]
                  (get-in rows [x y])))

    (defn init [vars hints]
        (if (seq vars)
            (let [hint (first hints)]
                (all
                    (if-not (zero? hint)
                        (== (first vars) hint)
                            succeed)
                                (init (next vars) (next hints))))
                                    succeed))

    (defn sudokufd [hints]
        (let [vars (repeatedly 81 lvar)
              rows (- vars (partition 9) (map vec) (into []))
              cols (apply map vector rows)
              sqs  (for [x (range 0 9 3)
                         y (range 0 9 3)]
                         (get-square rows x y))]
                    (run 1 [q]
                        (== q vars)
                        (everyg #(infd % (domain 1 2 3 4 5 6 7 8 9)) vars)
                        (init vars hints)
                        (everyg distinctfd rows)
                        (everyg distinctfd cols)
                        (everyg distinctfd sqs))))

    ;; ====

    (comment
    (sudokufd
        [0 0 3  0 2 0  6 0 0
         9 0 0  3 0 5  0 0 1
         0 0 1  8 0 6  4 0 0
         0 0 8  1 0 2  9 0 0
         7 0 0  0 0 0  0 0 8
         0 0 6  7 0 8  2 0 0
         0 0 2  6 0 9  5 0 0
         8 0 0  2 0 3  0 0 9
         0 0 5  0 1 0  3 0 0]))

[gist](https://gist.github.com/swannodette/3217582#file-gistfile1-clj)

[ClojureScript](https://github.com/clojure/clojurescript) compiles Clojure into Javascript which is guarenteed to be digestable by the [Goolge Closure](https://developers.google.com/closure/) compiler. While the ClojureScript implementation of core.logic is somewhat limited compared to the Clojure based one, you can still do some interesting things with it. If you are not familiar with ClojureScript you might want to check [this tutorial](https://github.com/magomimmo/modern-cljs) out. Some interesting examples of using canvas / SVG with ClojureScript, can be found [here](https://github.com/rm-hull/programming-enchiladas#examples)

Full Disclosure:  I am receiving a free GOTO ticket from the producers in exchange for blogging about the conference.
