# Responsive Web Design and Regular Expressions

Links:

1. [RegExr](https://regexr.com/)
2. [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
3. [Regex 101](https://regex101.com/)
4. [CSS Grid Reference](https://css-tricks.com/snippets/css/complete-guide-grid/)
5. [Responsive design with CSS Grid](https://medium.com/samsung-internet-dev/common-responsive-layouts-with-css-grid-and-some-without-245a862f48df)

## Regular Expression cheatsheet

**Character classes**
.	any character except newline
\w \d \s	word, digit, whitespace
\W \D \S	not word, digit, whitespace
[abc]	any of a, b, or c
[^abc]	not a, b, or c
[a-g]	character between a & g

**Anchors**
^abc$	start / end of the string
\b \B	word, not-word boundary

**Escaped characters**
\. \* \\	escaped special characters
\t \n \r	tab, linefeed, carriage return

**Groups & Lookaround**
(abc)	capture group
\1	backreference to group #1
(?:abc)	non-capturing group
(?=abc)	positive lookahead
(?!abc)	negative lookahead

**Quantifiers & Alternation**
a* a+ a?	0 or more, 1 or more, 0 or 1
a{5} a{2,}	exactly five, two or more
a{1,3}	between one & three
a+? a{2,}?	match as few as possible
ab|cd	match ab or cd

## Grid Layout

It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. You work with Grid Layout by applying CSS rules both to a parent element (which becomes the Grid Container) and to that element’s children (which become Grid Items)



[Back to Homepage](https://ashcaz.github.io/reading-notes)

