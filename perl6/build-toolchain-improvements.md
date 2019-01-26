Improve the Rakudo CI toolchain
==================================

Description
-----------

The MoarVM and Rakudo CI toolchains on GitHub (using Travis CI and AppVeyor)
could have a number of enhancements added. Here are three things in particular:
  * Code coverage: There is some automation of MoarVM coverage reports when running
    the NQP test suite [here](https://github.com/MoarVM/coverage), but that could be expanded to include
    results from running the Rakudo test suite as well a Roast spectest. Additionally,
    Rakudo can produce coverage reports of its code, that would also make sense to automate
    for its test suite and a Roast spectest.
  * Benchmarking: There are [some](http://moarvm.com/measurements/perl6-bench/) that run every day, but they have been broken
    for about two years. They could be fixed, as well as adding in something like https://github.com/japhb/perl6-bench.
  * Regression tests: [Blin](https://github.com/perl6/Blin) could be run automatically (e.g., at every NQP bump, every 10 or so Rakudo commits).
    


Expected outcomes
-----------------

Some/All of the above ideas (or new ones) added to the automated CI toolchains for MoarVM/NQP/Rakudo.


Required skills
---------------

Perl 6


Rating
------

Medium


Possible mentors
----------------

One of the Perl 6 list of mentors. (While I wouldn't mind helping out if possbile, I won't have the time/availability to be an official mentor this year.)
