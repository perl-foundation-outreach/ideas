DBD::MariaDB Prepared Statements, Async, Test Suite
===================================================

Description
-----------

[DBI](https://metacpan.org/pod/DBI) is a database independent interface for the Perl 5 language. [MariaDB](https://mariadb.org/about/) is a popular SQL database server. [DBD::MariaDB](https://metacpan.org/pod/DBD::MariaDB) is a DBI driver which allows Perl 5 DBI application to connect to a MariaDB or MySQL server. DBD::MariaDB is a fork of the older [DBD::mysql](https://metacpan.org/pod/DBD::mysql) driver that aims to have a full and correct Unicode support, fixed bugs which were not possible to fix in the DBD::mysql due to compatibility reason and also support for a new MariaDB specific features which are not available in the original MySQL software. DBD::MariaDB driver is developed in [GoodData](https://www.gooddata.com/) and its project page is on [GitHub](https://github.com/gooddata/DBD-MariaDB).


Expected outcomes
-----------------

There are several areas for improving the DBD::MariaDB driver. To call the project successful, at least one of the first two improvements must be completed.

- Implement a full support for server side prepared statements, including bind parameters, output parameters, multiple result sets and support for the MariaDB specific extension [execute direct](https://mariadb.com/kb/en/library/mariadb_stmt_execute_direct/). Currently DBD::MariaDB uses its own code for a placeholder replacement. Basic support for a server side prepared statements needs to be explicitly enabled.
- Implement an asynchronous / non-blocking mode of a query execution and server side prepared statements via the new MariaDB asynchronous [Non-blocking library API](https://mariadb.com/kb/en/library/non-blocking-client-library/). Currently DBD::MariaDB has a very limited and mostly buggy support for an asynchronous mode which uses undocumented functions provided by the MySQL client library.
- Extend and fix an existing driver test suite. Currently DBD::MariaDB tests do not cover all DBI application use cases, some tests are missing, other tests are incorrectly written. Proper tests are needed for ensuring the compatibility between the MariaDB server and a DBI client application, i.e. that everything implemented in the DBD::MariaDB driver works as expected. Tests are now automatically running on [Travis CI](https://travis-ci.org/gooddata/DBD-MariaDB/branches) and [AppVeyor](https://ci.appveyor.com/project/gooddata/dbd-mariadb/branch/master) services for every change in the driver.


Required skills
---------------

Experience with C, Perl and SQL languages.


Rating
------

Medium.


Possible mentors
----------------

- Pali (pali@cpan.org / [CPAN](https://metacpan.org/author/PALI) / [GitHub](https://github.com/pali))
- Choroba (choroba@cpan.org / [CPAN](https://metacpan.org/author/CHOROBA) / [GitHub](https://github.com/choroba))

