LGrind - a source pretty printer for LaTeX
==========================================

A pretty printer for various programming languages (using LaTeX).
Current version: 3.68

Welcome to LGrind. LGrind is a descendant of the Unix utility vgrind. It is
used to produce a beautified version of your source code using LaTeX. Unlike
other packages this is not pure TeX but an external preprocessor. You run e.g.

    lgrind example.c > example.tex
    latex example.tex

to get a complete listing. Options for producing includable files and pro-
cessing embedded listings in LaTeX texts are provided.


What you need: (Installation part 2)
------------------------------------

- `lgrind`      – (or `lgrind.exe`) just where you like it
- `lgrind.sty`  – somewhere in LaTeXs reach
- `lgrindef`    – anywhere; (position is semi-fixed in the executable)
- LaTeX2e       – the obsolete LaTeX 2.09 is not supported
- LGrind utilizes by default the fancyhdr package by Piet van Oostrum. You
  can change this behaviour by modifying the lgrindef file.


How to get these files: (Installation part 1)
---------------------------------------------

- If your executable is not provided, all the  source files are in the source
  directory, a makefile provided.
- Run LaTeX or TeX on lgrind.ins. You will obtain lgrind.sty.
- Or simply run make in the top directory. This also gives lgrind.sty


Documentation
-------------
Main documentation is in `lgrind.dtx`. Run LaTeX on lgrind.dtx and the result is
`lgrind.dvi`. There are also manpages `lgrind.1` and `lgrindef.5` for people who
prefer those, but notice that I am not always able to keep them up to date.
To right the wrong impression: parts of the documentation have been written
by my predecessors, my thanks to them.



Files in the directories:
-------------------------
`lgrind.ins`      DocStrip driver
`lgrind.dtx`      Documented package
`lgrind.gls`      Glossary and index for the documentation (for the ones with-
`lgrind.ind`        out MakeIndex, and because it had to be modified by hand)
`lgrindef`        The language definition file


In the directory `source`:
`lgrind.c`        The source code for the LGrind executable
`lgutil.c`
`lgrindef.c`
`lgrindef.h`
`regexp.c`
`regexp.h`
`v2lg.c`          Source code for verbatim to embedded source converter
`retest.c`        Test program for the regular expression routines
`lgrind.1`        Man-pages for the LGrind program
`lgrindef.5`                and the language definition file
`Makefile`        Makefile for Unices
`makefile.dos`    Makefile for MS-DOS (not tested anymore)
`makefile.emx`    Makefile for use with DMAKE


In the directory `example`:
`c2tex.bat`       Example batch files for facilitating calls to LGrind
`asm2tex.bat`
`c2tex`           ditto as Bourne shell scripts
`asm2tex`
`egmasm.asm`      Example sources
`egcprog.c`
`subst`           Example substitution file
`lgrindeg.tex`    Example making use of the above



Comments, contributions, questions and cheques
----------------------------------------------
LGrind is generally licensed under BSD. However, LGrind contains non-free
code written by Van Jacobson, who does not answer to any request for changing
his licence (BSD with no-sell clause). This software is therefore not
maintained. I also do not accept any cheques anymore.

Have Fun!

