# guile-sicp-piclang
A Guile Scheme implementation of the Henderson-Escher picture language, as seen
in [Structure and Interpretation of Computer Programs Section
2.2.4](http://sarabander.github.io/sicp/html/2_002e2.xhtml#g_t2_002e2_002e4).
W.I.P.

This implementation makes it possible to run code examples from the book's
Picture Language section without having to implement much of the language
beforehand. Much of the code is courtesy of
[ProducerMatt](https://github.com/ProducerMatt/SICP-solutions) and all of it is
work in progress. In particular, a guix package recipe is to be added.

At the moment, the code gets you far enough to be able print the square limit of
a wave painter in repl. Invoke (paint-lines (square-limit wave 4)) to test.
