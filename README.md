git stale-branches
==================

List stale branches and display the removal commands without actually removing the branches.

A stale branch is a branch which has been remotely or locally merged.

Installation
============

In order to use the git-stale-branches script as a new subcommand with git, 
it needs to be available in your PATH.

Option 1
--------

Add the `git-stale-branches` directory to your `PATH`:

    export PATH=$PATH:~/git-stale-branches/bin

The additional git command can be used like any other git command.

E.g. to list all stale branches use:

    git stale-branches

To list stale branches for a specific remote:

    git stale-branches origin



Option 2
--------

Use the Makefile to copy the scripts to your `/usr/local/bin` directory.
This will also copy the man pages to the appropriate directories on your
system.

    make install

To remove the scripts and man pages run `uninstall`:

    make uninstall

Commands
========

* `git stale-branches` -> List all stale branches
* `git stale-branches REMOTE` -> Only consider the REMOTE remote

Credits
=======

Git plugin project template copied from https://bitbucket.org/ssaasen/git-pastiche.
