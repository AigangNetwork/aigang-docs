Documenation examples
=====================
Here lays are some examples for writing well-formated documentation

Code
----
This is a typical paragraph.  An indented literal block follows.

::

    for a in [5,4,3,2,1]:   # this is program code, shown as-is
        print a
    print "it's..."
    # a literal block continues until the indentation ends

This text has returned to the indentation of the first paragraph,
is outside of the literal block, and is therefore treated as an
ordinary paragraph.

Tables
------
+--------------+----------+-----------+-----------+
| row 1, col 1 | column 2 | column 3  | column 4  |
+--------------+----------+-----------+-----------+
| row 2        | Use the  |  tables   | more.     |
+--------------+----------+-----------+-----------+
| row 3        |          |           |           |
+--------------+----------+-----------+-----------+

Images
------
.. image:: ../img/logo-color.png

Hyperlinks
----------
This is a paragraph that contains `a link`_.

.. _a link: http://example.com/

Lists and emphasis
------------------
* one asterisk: *text* for emphasis (italics),
* two asterisks: **text** for strong emphasis (boldface), and
* backquotes: ``text`` for code samples.
