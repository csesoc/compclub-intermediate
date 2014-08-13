Recap of Python
===============

Python is a brilliant language (I say that as a totally unbiased observer). We
can do all sorts of things really easily, without having to know what the
computer is doing behind the scenes. That's the exact reason why Python is a
terrible programming language to learn programming with, but an excellent
choice to use forever after.

Printing
--------

    >>> print "Hello World"
    Hello World
    >>> my_string = "Hello World"
    >>> print my_string
    Hello World
    >>> first_name = "Bob"
    >>> last_name = "Smith"
    >>> print "Hello %s %s" % (first_name, last_name)  # this is an ugly line of code!
    Hello Bob Smith
    >>> print "Hello {first_name} {last_name}".format(first_name=first_name, last_name=last_name)
    Hello Bob Smith
