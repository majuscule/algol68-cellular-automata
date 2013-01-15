### How to run:

#### Install [ALGOL 68G](https://en.wikipedia.org/wiki/ALGOL_68G) from your package manager or [source](http://jmvdveer.home.xs4all.nl/algol.html)

#### Run with the interpreter
- `a68g cellular_automata.a68`

#### Or compile and run
- `a68g --compile cellular_automata.a68`

- note from `A68G 1`
>     --compile | --no-compile
>             Switch compilation of units on or off. Compilation omits many of the runtime checks offered by the
>             interpreter proper. The program is not executed and a shell script is generated combining source code
>             and its shared library. This shell script can be used as a pseudo-executable.

- note from me:
```
    $ file cellular_automata.sh
    cellular_automata.sh: data
    $ head -n3 !$
    head -n3 cellular_automata.sh
    #! /usr/bin/a68g --run-script
    cellular_automata
    --verify "algol68g 2.6"
```
