.. |labmodule| replace:: 1
.. |labnum| replace:: 1
.. |labdot| replace:: |labmodule|\ .\ |labnum|
.. |labund| replace:: |labmodule|\ _\ |labnum|
.. |labname| replace:: Lab\ |labdot|
.. |labnameund| replace:: Lab\ |labund|

Lab |labmodule|\.\ |labnum|\: Playing with reStructedText \(rST)
----------------------------------------------------------------

********
Titles
********

Titles can be created in two ways, underlines and under/over lines. The lines must be >= the length of the title itself.  Additionally, both under and over lines must be equal.

===================
More about Titles
===================

The special characters you can use for title lines are as follows:

* # with overline, for parts
* \* with overline, for chapters
* =, for sections
* -, for subsections
* ^, for subsubsections
* “, for paragraphs

******
Lists
******

Lists can be bulleted or numbered.  Numbered lists can be static or dynamic.

* This is a bulleted list.
* It has two items, the second
  item uses two lines. (note the indentation)

This list is a statically numbered list.

1. This is a numbered list.
2. It has two items too.

This list is a dynamically numbered list using the #. command

#. This is a numbered list.
#. It has two items too.

**************
Inline markup
**************

In rST, you can use inline markup commands. The standard reST inline markup is quite simple to use:

* one asterisk: *text* for emphasis (italics)
* two asterisks: **text** for strong emphasis (boldface), and
* backquotes: ``text`` for code samples.

************
Line Spacing
************

| Similar to HTML, spacing between lines isn't represented on the page once loaded.  Unlike HTML, I have yet to find a way to insert a break with a flag such as <br>.  Line Blocks are the closest thing I have been able to find. To create a line block simply add a pipe "\|" with a following space before your text.
|
| Line 1
| Line 2
|
| Line 4

********
Tables
********

.. list-table::
    :widths: 20 40 40
    :header-rows: 1
    :stub-columns: 1

    * - **Column one**
      - **Column two**
      - **Column three**
    * - Column one row one
      - - **Column two:** item one
        - **Column two:** item two
      - Column three/*in italics*
    * - Column two row two
      - - **Column two:** item one
        - **Column two:** item two
      - Column three/*in italics*

**Highlighted Instructions**

::
    POST https://{{big_ip_a_mgmt}}/mgmt/tm/ltm/pool


*******
Images
*******

   |image1|

************
Sphinx
************

http://www.sphinx-doc.org/en/stable/tutorial.html

***************
rST Cheet Sheet
***************

https://github.com/ralsina/rst-cheatsheet/blob/master/rst-cheatsheet.rst
