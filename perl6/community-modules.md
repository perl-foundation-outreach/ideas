Upgrade high-priority community modules
==================================

Description
-----------

Some modules in the Perl 6 ecosystem have
been
[adopted by the community](https://github.com/perl6-community-modules/) due
to different reasons, inclusing donation by the original author. In
many cases, they are modules used extensively by other modules and
form the foundation of many applications; however, since they are
community-maintained, there's not single author paying attention to
them all the time.

In this project we will take into
account
[River scores](https://github.com/JJ/p6-river/blob/master/data/river-scores.csv) to
select modules that many other modules depend upon, and upgrade them
by

* Fixing bugs
* Adding tests to make them follow specs.
* Improve performance.


Expected outcomes
-----------------

Modules to be considered:

* [URI](https://github.com/perl6-community-modules/uri) is the one
  with the highest River score, meaning there are many modules that
  depend on it. There are 3 issues now. This module should be upgraded
  and released as a (stable) version 1.0, which should include passing
  all tests that other, up-to-date modules like Perl5's URI include.
  
* [Pod::To::HTML](https://github.com/perl6/Pod-To-HTML) converts Pod
  to HTML, and could be part of the [project to revamp documentation
  tooling, since it's used extensively there](https://github.com/perl6/Pod-To-HTML),
  although it stands by itself. There are 7 issues now, these issues
  should be addressed, and this module released to a (stable) version
  1.0.
  
* [Test::When](https://github.com/perl6-community-modules/perl6-Test-When) this
  module was recently adopted, and it's got 0 issues. However, it
  mentions restrictions that are not implemented and needs some
  adaptation of the documentation. It's at version 1.001, should be
  upgraded and version 1.002 released.

* [LWP::Simple](https://github.com/perl6/perl6-lwp-simple), a simple
  HTTP client which is right now at version 0.1. It has 3 issues,
  which should be addressed and solved, and release a stable version
  1, which should include all the features of the equivalent Perl5's
  LWP::Simple. 
  
Modules requested, or wanted, by the community are listed
in
[this repo](https://github.com/perl6/perl6-most-wanted/blob/master/most-wanted/modules.md). Some
of them are work in progress, but some of them could be really
interesting to have, for instance, a Term::UI module for creating
terminal user interfaces.

Required skills
---------------

Knowledge, or willing to learn, Perl 6, including handling Perl 6 grammars.


Rating
------

Medium. 


Possible mentors
----------------

JJ Merelo.
