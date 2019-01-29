# Encoding/Decoding

This idea involves file encodings. File encodings are decoded and encoded in MoarVM. Most of the work
will be in C, whoever takes on the project should know C. Knowing Perl or Perl 6 is not a hard requirement.

Ideas would be one or both of the following:

## Refactoring the Decode/Decodestream code

Currently we have duplicated logic for decoding static data compared to decoding a "stream" i.e.
one segment at a time of indefinite length. We would like to get to the point that there is one
logic path which handles the encoding, and some wrapper code is able to handle the differences
between decode/decodestream without caring about the format involved.

## Implementing the GB2312 Encoding (Simplified Chinese)

This encoding is the most commonly used one which we do not yet have the ability to encode or decode.
Implementing this does not involve knowing how to read or write simplified chinese, and is focused
on implementing the standard into our codebase.


## Mentor

Samantha McVey (samcv) is able to be a mentor for either of the two above mentioned projects.
