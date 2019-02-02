Implementing the GB2312 Encoding (Simplified Chinese) [README.md](README.md))
==================================

Description
-----------

This idea involves file encodings. File encodings on Perl 6 are decoded and encoded in MoarVM. 


This encoding is the most commonly used one which we do not yet have the ability to encode or decode.
Implementing this does not involve knowing how to read or write simplified chinese, and is focused
on implementing the standard into our codebase.


Expected outcomes
-----------------

MoarVM should be able to decode and encode GB2313 algorithm by the end of the project.

Required skills
---------------

Most of the work
will be in C, whoever takes on the project should know C. Knowing Perl or Perl 6 is not needed.


Rating
------

Medium

Possible mentors
----------------

Samantha McVey (samcv) is able to be a mentor for either of the two above mentioned projects. Can be
reached at samantham@posteo.net or on Freenode as samcv.


Improving Decoding Modularity
==================================

Description
-----------

This idea involves file encodings. File encodings on Perl 6 are decoded in MoarVM. At the moment we have separate sections of code
for handling decoding of static data and a separate path for decoding a stream of data. This project involves unifying
the two sets of code to make it easier to add further encodings and reduce tha chance of differences between the two code
paths. If attempting this project it is highly recommended to first have implemented a new encoding themself to familiarize themself with the codebase.


Expected outcomes
-----------------

Expected that the student creates a common code path that stream and non stream decoding can use,
with the only difference being the outside loop calling the processing function.

Nice to have: the student identifies common data that must be stored between iterations of
the file decoding process, allowing different file encodings to reuse the outer loops.


Required skills
---------------

Most of the work
will be in C, whoever takes on the project should know C. Knowing Perl or Perl 6 is not needed.


Rating
------

Medium Hard

Possible mentors
----------------

Samantha McVey (samcv) is able to be a mentor for either of the two above mentioned projects. Can be
reached at samantham@posteo.net or on Freenode as samcv.

