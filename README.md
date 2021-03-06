What's Ruby
===========

Ruby is the interpreted scripting language for quick and easy
object-oriented programming. It has many features to process text files
and to do system management tasks (as in Perl). It is simple,
straight-forward, and extensible.

Features of Ruby
----------------

-   Simple Syntax
-   *Normal* Object-Oriented features(ex. class, method calls)
-   *Advanced* Object-Oriented features(ex. Mix-in, Singleton-method)
-   Operator Overloading
-   Exception Handling
-   Iterators and Closures
-   Garbage Collection
-   Dynamic Loading of Object files(on some architecture)
-   Highly Portable(works on many UNIX machines, and on DOS, Windows,
    Mac, BeOS etc.)

-   How to get Ruby

The Ruby distribution can be found on:

ftp://ftp.ruby-lang.org/pub/ruby/

You can get it by anonymous CVS. How to check out is:

    $ cvs -d :pserver:anonymous@cvs.ruby-lang.org:/src login
    (Logging in to anonymous@cvs.ruby-lang.org)
    CVS password: anonymous
    $ cvs -z4 -d :pserver:anonymous@cvs.ruby-lang.org:/src checkout ruby

Ruby home-page
--------------

The URL of the Ruby home-page is:

http://www.ruby-lang.org/

Mailing list
------------

There is a mailing list to talk about Ruby. To subscribe this list,
please send the following phrase

    subscribe YourFirstName YourFamilyName

e.g. subscribe Joseph Smith

in the mail body (not subject) to the address
<ruby-talk-ctl@ruby-lang.org>.

How to compile and install
--------------------------

This is what you need to do to compile and install Ruby:

1.  If ./configure does not exist or is older than configure.in, run
    autoconf to (re)generate configure.

2.  Run ./configure, which will generate config.h and Makefile.

3.  Edit defines.h if you need. Probably this step will not need.

4.  Remove comment mark(\#) before the module names from ext/Setup (or
    add module names if not present), if you want to link
    modules statically.

    If you don't want to compile non static extension modules (probably
    on architectures which does not allow dynamic loading), remove
    comment mark from the line "\#option nodynamic" in ext/Setup.

5.  Run make.

6.  Optionally, run 'make test' to check whether the compiled Ruby
    interpreter works well. If you see the message "test succeeded",
    your ruby works as it should (hopefully).

7.  Run 'make install'

    You may have to be a super user to install ruby.

If you fail to compile ruby, please send the detailed error report with
the error log and machine/OS type, to help others.

Copying
-------

See the file COPYING.

The Author
----------

Feel free to send comments and bug reports to the author. Here is the
author's latest mail address:

    matz@netlab.jp

------------------------------------------------------------------------

    created at: Thu Aug 3 11:57:36 JST 1995
    Local variables:
    mode: indented-text
    end:
