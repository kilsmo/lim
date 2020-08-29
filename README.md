# Lim

Lim is a new programming language.

Do we really need another programming language? No, we don't, but I do. I want to do code analysis for a problem that I find very
interesting, and that I think will be very useful if it is solved. I need a limited programming language  (Lim) to be able to make
the code analysis a bit simpler, and that is why this project was started. I have no ambition to make lim into a popular programming
language.

So, what kind of language is Lim? Lim is a pure, synchronous, functional language, that can be transpiled into JavaScript. It is meant
to be used together with other languages that transpiles into JavaScript, since you can't make a complete application with it.

Since the reason for Lim is code analysis of a specific problem, there would be no real need to care about syntax and such. But, when
you actually get a chance to design a programming language, why not have fun and try to be at least a little bit original.

A *.lim file starts with any number of imports followed by any number of top level functions.

An import line looks like this: sort, map : 'underscore'

An exported function looks like this: foo(x, y)

A private function looks like this: _bar(x, y, z)

There are no keywords used in Lim. This is how you write if/else if/else code:

```
? a <= 3
  3
? a >= 5
  5
: 4
```

Every expression returns a value, and the last expression is a function is always returned.

This is how you make an explicit return in Lim: => 3

Variables can never change (they are like constants: a = 3 (can't change a anymore)

Indentation is used for blocks, and also for line continuations. A line can be continued anywhere it is not finished (like a paranthesis that hasn't been closed)

A limited set of operators from JavaScript is used. (some disappears naturally since varaiables can't be changed)

You can define unnamed functions inside a function like sort: (a, b) a > b

That was a very quick tour of the Lim language. Implementation of the language is pending.
