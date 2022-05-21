# Instructions Part 1

## challenges01.4th

This files tests your understand of stack manipulation instructions. You'll find a a number of incomplete word definitions like so:

```
: challenge1 ( 1 2 3 - 1 2 )
    ( your code ) ;

T{ 1 2 3 challenge1 -> 1 2 }T
```

The stack notation next to each word tells you what is on stack and what should be on stack after your word is run.

Your challenge is to replace `( your code )` with Forth stack instructions (`dup`, `swap`, `tuck`, `nip`, etc.). To check your solutions, simply run:

```bash
$ make check1
```

The included makefile will run the tests. If there are no errors reported, congratulations! You passed this challenge.

Some of these examples are taken from the [Gforth Tutorial][gforthtut].

## challenges02.4th

In this challenges, you'll define some stack manipulation words of your own. You'll use the five basic words `swap`, `rot`, `dup`, `drop`, and `over` to define common other words like `tuck` or `nip`.

This is actually how you build more complex Forth programs: You define more complex words step by step from simpler ones. This is often referred to as [bottom-up programming](http://www.paulgraham.com/progbot.html).

Your challenge is to replace `( your code )` with words to emulate the behavior described in the stack effect notation.

```bash
$ make check2
```

Ignore the warnings Gforth prints; replacing and redefining the original word definitions is exactly the point of this challenge.

[gforthtut]: https://www.complang.tuwien.ac.at/forth/gforth/Docs-html/Stack-Manipulation-Tutorial.html#Stack-Manipulation-Tutorial
