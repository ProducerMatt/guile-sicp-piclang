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

Functions that the book expects you to implement are implemented here as
`foo-answer`. When defining your own versions, keep in mind that to test a
function that uses your version of something, you need to redefine the function
also, otherwise it will use the functions within the module itself. In other
words, if you want to define the function below, in order to make the function
square-limit care about your below, you need to also redefine square-limit to
use your version of below.

At the moment, the code gets you far enough to be able print the square limit of
a wave painter in repl. Invoke `(paint-lines (square-limit wave 4))` to test.

To use the module, download sicp-piclang.scm, load it into your repl and invoke
`(use-modules (sicp-piclang))`
