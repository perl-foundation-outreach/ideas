Testing JIT compilation and runtime specialization in MoarVM
==================================

Description
-----------

Currently, MoarVM is tested indirectly via the NQP and Rakudo test
suites. This is not necessarily sufficient to test the `spesh` and JIT
subsystems of MoarVM, because these:

- operate only on very active code, which is rare in short-running tests
- work on an asynchronous thread, which makes this (somewhat) unpredictable
- are many layers removed from the code-as-written (separated by the
  rakudo/nqp bytecode compiler and static optimizer)

Yet these are highly complex subsystems with strict correctness
requirements. Therefore we need a system to test these directly.

Expected outcomes
-----------------

A succesful project will deliver:

- A tool to execute test cases for `spesh` and the JIT compiler. This
  tool should read a test case and directly build a suitable IR
  representation of the code to be processed.
- A few example test cases that exercise this system.


Required skills
---------------

A student with skills in C programming and a working understanding of
virtual machines and compilers should have a good chance of
succeeding.


Rating
------

Medium/hard


Possible mentors
----------------

[Bart Wiegmans](https://github.com/bdw) (bartwiegmans@gmail.com)
