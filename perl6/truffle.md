Truffle/GraalVM backend
=======================

Description
-----------

We have an initial start of an [attempt](https://github.com/perl6/nqp/tree/truffle) that passes some NQP tests and will be expanded as part of the project.
[Truffle](https://github.com/oracle/graal/tree/master/truffle) already has implementations for varied programming languages and after initial experimentation seems to be an almost perfect fit for Perl 6.
The project will involve expanding the Truffle annotated interpreter for a processed QAST (intermediate tree representations of that NQP/Perl 6 use).
Assistance in regards on obscure details of the QAST representation however will be provided.
Code from the JVM backend also can get reused for some of the primitives.

Expected outcomes
-----------------

Preferably getting NQP (a Perl 6 subset the Rakudo compiler is running itself) running on truffle to compile itself. Getting a large subset of NQP functionallity working on truffle and benchmarking it and testing out integration with other languages would also be an acceptable result.

Required skills
---------------

Knowledge of Java and the willingness to understand how the fairly complicated Truffle framework works.

Rating
------

hard


Possible mentors
----------------

Paweł Murias (pawelmurias@gmail.com)
