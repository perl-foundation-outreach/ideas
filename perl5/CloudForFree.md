CloudForFree 
==================================

Description
-----------

This project relates to development of the CloudForFree.org software:

http://cloudforfree.org/

https://github.com/wbraswell/cloudforfree.org

The CFF platform is based on ShinyCMS on top of Perl Catalyst, combined with RPerl and CGI::Ajax and Ace editor, etc.

Expected outcomes
-----------------

Completion of any or all of the following objectives will be considered a success for this project.

Phase 1, Terminal Emulation
- Full xterm Terminal Emulation For Command-Line Job Execution
- Includes All VT100 & VT102 & VT220 Features
- Resize Number Of Rows & Columns By Window Resize
- Resize Font Size By User Configuration
- Backspace, Tab, Other Special Command Characters
- Arbitrary Placement Of Characters At Any Row & Column
- Color Characters & Background
- Curses & Other Menu Support
- Full Window (F10) & Full Screen (F11)

Phase 2, Graphical Output & Mouse Input
- Full X-Windows Graphics Output Using Xpra HTML5 Client
- Generate Output Using SDL From Perl & C
- Mouse Left-Click, Right-Click, Drag, Scroll
- Resize Number Of Available X & Y Pixels By Window Resize
- Full Window (F10) & Full Screen (F11)

Phase 3, GitHub Repositories Integration
- Import & Setup User's GitHub Keys Via Linux User Account
- List Of All GitHub Repos With User As Owner Or Collaborator
- Admin Mode, Display All Repos
- Allow User To Enter Any Other Readable GitHub Repo URL
    ex. https://github.com/wbraswell/physicsperl
- Buttons For Basic User Git Commands
    clone    add    commit    push    pull    checkout    status
- Do Not Duplicate Any GitHub Web Functionality

Phase 4, Job Queue
- Job Scheduler & Monitor Using OAR (1st Choice), Or HTCondor Or Slurm (2nd Choices)
- Manage User's Jobs Via Linux User Account
- List Of All Current Jobs With User As Owner
- Admin Mode, Display All Jobs
- FileManager For Selecting *.pl RPerl Programs To Run
- Buttons For Basic Job Control Commands
    start    restart
    stop (SIGTERM)    force stop (SIGKILL)    pause (SIGSTOP)    continue (SIGCONT)
    show/hide CLI (From Phase 4)    show/hide GUI (From Phase 5)
- Display Resources: FLOPS, Cores, Memory, Storage; Total, Unused, Available To User


Required skills
---------------

Programming and system administration skills will be required in one or more of the following areas:

Linux
Ubuntu
GitHub
Perl
Catalyst
C++

Rating
------

Medium

Possible mentors
----------------

Will 'the Chill' Braswell
william.braswell@autoparallel.com
