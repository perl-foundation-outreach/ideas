Linking Perl 6 Compiler and Programs
==================================

Description
-----------

Currently, starting a Perl 6 programs means loading a shell script
that starts a MoarVM, that loads the rakudo compiler (as bytecode) and
libraries (also bytecode), before loading the user script and
compiling that. This adds significantly to the startup time of perl6
programs, is fragile and nonportable (the paths of MoarVM and the
rakudo compiler are hardcoded) and breaks tool support (for example,
`gdb perl6 foo.pl6` does not work). We want to make that better by
making `perl6` a direct executable, and if possible, user programs as
well.

Expected outcomes
-----------------

This project would have two main goals:

- `perl6` would be a single, self-contained executable, much like
  `perl` is. Thus running `perf perl6`, `gdb perl6`, `valgrind perl6`
  should 'just work'.
- `perl6 --compile foo.pl6` would generate an executable that would
  be, to some reasonable degree, self-contained so that it could be
  used for binary distributions.

Details
-------

For MoarVM, there are several options to achieve this. One
particularly interesting option is to package MoarVM bytecode in the
[ELF](https://en.wikipedia.org/wiki/Executable_and_Linkable_Format)
file format (on linux). This is similar to what
[guile scheme](https://wingolog.org/archives/2014/01/19/elf-in-guile)
does and has numerous advantages:

- ELF is well documented and has broad platform and toolchain
  support. (For instance, see the
  [debug/elf](https://golang.org/pkg/debug/elf/) package in the golang
  standard library). It may be possible to use the system linker.
- ELF supports many useful features (for instance, it's possible to
  refer to an interpreter, avoiding the need to directly link the
  MoarVM executable)
- Sections of the ELF file may be shareable between instances of the
  VM, reducing memory load. (This depends on the loading strategy).

A downside is that this would only work on linux/BSD etc, not on macOS
or Windows. That is acceptable as a proof-of-concept.

There are certainly other options possible. For instance, another
option that has been discussed it to compile the MoarVM bytecode for
the rakudo compiler to a header and use that to compile a loader
program in C. However, this would require the user to have a C
compiler installed for `perl6 --compile` to work. (That may be an
acceptable tradeoff).

Because this is a large and technically challenging project, a student
is highly adviced to do some research and figure out what they feel
confident in being able to deliver. Students are also encouraged to
explore and propose other implementation options. Although this
description been written with MoarVM in mind, students that would like
to work on a solution for the JVM backend are also welcome to apply.

Required skills
---------------

A student is more likely to succeed having a good knowledge of C and a
working knowledge of dynamic linking and loading.


Rating
------

Medium/hard, depending on strategy

Possible mentors
----------------

[Bart Wiegmans](https://github.com/bdw) (bartwiegmans@gmail.com), brrt on freenode
