Perl 5: Dancer2 Configuration Improvements
==========================================

Description
-----------

A survey run by the Dancer Core team in 2017 showed that a number of Dancer2 developers felt that application configuration could be improved. Some
mistakes were made in trying to make the configuration of Dancer2 applications more flexible, and even more mistakes made trying to fix the earlier
issues. An expandable configuration is needed, allowing developers to choose the method of configation that best suits them.


Expected outcomes
-----------------

* Make the configuration system pluggable, much like sessions and templates in Dancer2 currently are.

* Package the existing configuration system up as a plugin to the new configuration engine. Ship in the default Dancer2 installation.

* Document and test the new configuration engine. Include a walkthrough of creating a new configuration plugin.

* Create a base set of simplified configuration systems: YAML only, JSON only, hash only. Document and test.


Required skills
---------------

Experience with Perl 5 and Moo/Moose is required. Dancer/Dancer2 experience is preferred but not necessary.


Rating
------

Hard


Possible mentors
----------------

* Jason Crome (cromedome): [CPAN](https://metacpan.org/author/CROMEDOME)/[GitHub](https://github.com/cromedome)/jason@crome-plated.com


