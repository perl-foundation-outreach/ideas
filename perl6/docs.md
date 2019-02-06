Perl documentation tools
========================

Description
-----------

Perl 6 documentation uses different tools to index, process and
generate HTML pages (and other formats). What can be said now about
the tooling is that it's working, but little else.

In the Perl 6 documentation community we are right now in a process of
redesign and overhaul of the whole documentation system that includes

* Specifications of documentation page, how source content and
  metadata are going to be processed and indexed.
  
* Specifications of document collections page, that allow easy
  navigation, but also fast regeneration in case of change.
  
* Refactoring of the perl6 documentation tool, p6doc, which is used
  for visualizing the Perl documentation.
  
* Tests and tools for the specificacions above.

* Optimization of tests documentation must pass with respect to
  content and also fulfillment of specs.

The perl documentation tools are right now in a state of flux. There's
[new specification](https://github.com/perl6/doc/wiki/Document-file-specification) right
now, but it needs to be fleshed out and implemented. There are also
several issues that need to be addressed, involving the spinning off
of different modules that are now included in the documentation repo.


Expected outcomes
-----------------

* Input and feedback into the specificactions.
* Creation of tests for the specifications.
* Creation of an indexing and content generation tool according to the
  specifications.
* Help with refactoring existing tools and a easy migration path from
  existing infrastructure.
* Contribution to documentation content in the parts that are right
  now lacking.


Required skills
---------------

Required or prefered skills the student should have to be able to
tackle this project.

* Some experience with Perl 6 is appreciated, but not really
  needed. Will to learn will be a requisite.
* Experience with grammars and language parsing.


Rating
------

Medium.


Possible mentors
----------------

[JJ Merelo](https://github.com/JJ), [Richard Hainsworth](https://github.com/rhainsworth), [Tom Browder](https://github.com/tbrowder).
