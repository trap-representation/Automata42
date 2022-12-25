Automata42
----

![Automata42 logo](./logo-github-light.png#gh-light-mode-only)
![Automata42 logo](./logo-github-dark.png#gh-dark-mode-only)

This is Automata42 - a language for defining state machines.

The implementation of Automata42 I'm working on is called Simple42. As of now, Simple42 translates the source file to C; however, in the future I do have plans on adding more translation targets (including [Chlore](https://github.com/trap-representation/Chlore)).

I will rewrite Simple42 in Chlore soon, and open-source the project, but as of now, the only things you'll be able to find in this repository are random examples, but I hope they're enough to give people a feel of what the language is like.

Automata42 has a (WIP) specification too, link to which will ofcourse be put here in the next few months.

Automata42 is complete enough to be able to perform lexical analysis on Automata42 source files. Such a lexical analyzer can be found in `examples/example0.a42`; it writes all the tokens (but keywords, which I have plans on adding support for in the future) it finds to stdout, and if the source file ends in a partial token, it exits with an exit code of 1.

The reason I built this before rewriting the MChlore translator entirely in Chlore, is because I wanted to generate a lexical analyzer with Automata42 for Chlore, even though I have hand-written one already - because why not.
