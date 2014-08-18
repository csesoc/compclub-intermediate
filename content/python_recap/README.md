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
    >>>

Maths
-----

    >>> 2 - 0
    2
    >>> 2 - 1
    1
    >>> 2 - 3
    -1
    >>> 2 * 2
    4
    >>> 2 ** 3
    8
    >>> 10 + 2
    12
    >>> 20 / 4
    5
    >>> 12 % 5  # this is the modulo operator
    7

Comparisons
-----------

    >>> print 1 == 1
    True
    >>> print 1 == 2
    False
    >>> print "string a" == "string b"
    False
    >>> print 3 <= 3
    True
    >>> print 3 < 3.5
    True
    >>> print 3 < 7/2  # muahahaha, sneaky integer division
    False
    >>> print 3 < 7.0/2
    True

Loops
-----

    >>> my_string = "Hello!"
    >>> for c in my_string:
    ...     print c
    H
    e
    l
    l
    o
    !
    >>> for i in range(10):
    ...     print i
    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    >>>

Fun datatypes
-------------

    >>> my_tuple = (3, 5, 7, 11, 13)
    >>> print my_tuple
    (3, 5, 7, 11, 13)
    >>> my_other_tuple = ('string', 'o', 'r', 'letters', 'or', 'numbers!', 1, 2, 7.5, 3.14159)
    >>> print my_other_tuple
    ('string', 'o', 'r', 'letters', 'or', 'numbers!', 1, 2, 7.5, 3.14159)
    >>> my_list = ['a list is', 'like a tuple', "but we're allowed", "to change", "things"]
    >>> print my_list
    ['a list is', 'like a tuple', "but we're allowed", 'to change', 'things']
    >>> my_list[0] = "Python lists"
    >>> my_list[-1] = "the indices"
    >>> print my_list
    ['Python lists', 'like a tuple', "but we're allowed", 'to change', 'the indices']

    >>> my_dictionary = {'Harry Potter': 'Gryffindor', 'Zacharias Smith': 'Hufflepuff', 'Draco Malfoy': 'Slytherin'}
    >>> print my_dictionary['Harry Potter']
    Gryffindor

Functions
---------

    >>> def print_square(n):
    ...     print n**2
    >>> print_square(2)
    4
    >>> print_square(3)
    9
    >>> def return_square(n):
    ...     return n**2
    >>> two_squared = return_square(2)
    >>> print two_squared
    4
    >>> def factorial_recursive(n):
    ...     if n == 1:
    ...         return 1
    ...     else:
    ...         return n * factorial_recursive(n-1)
    >>> five_factorial = factorial_recursive(5)
    >>> print five_factorial
    120
    >>>

I can't be bothered writing any more, here are some questions for revision
--------------------------------------------------------------------------
### Maths
* BODMAS -- what happens if I do
    * 5 + 3 * 6
    * (5 + 3) * 6

TODO put more questions here. Preferably things that can be abused with pythonic stuff like....

* Print even numbers between 0 and 10 in only one line: `print ' '.join([x for x in range(10) if x % 2 == 0])`

### Challenge
* Given a list of numbers between 0 and 100 (inclusive), print out the ranges of numbers that are missing.
    e.g. given [4, 10, 11, 50] print out "0-3, 5-9, 12-49, 51-100". Note -- this has more edge cases than it would seem at first.
