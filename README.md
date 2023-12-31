# (C)ian's (Mark)up

Personal markup language.

## Headers

Headers start with a =.  
The = must be followed by a space.  
There are 6 layers of headers, same as HTML.  
```
= Level 1
== Level 2
=== Level 3
==== Level 4
===== Level 5
====== Level 6
```

## Lists

### Unordered Lists

All unordered lists begin with a -.  
Sublists are also possible.  
```
- Item
	- Sub-Item
		- Sub-sub-Item
	- Sub-Item
- Item
```

### Ordered Lists

Ordered lists begin with a +.  
Sublists are also possible.  
```
+ Item
	+ Sub-Item 
		+ Sub-Sub-Item
	+ Sub-Item
+ Item
```

## Inline Markup

The following rules count for all inline markup:
1. The begin delimeter must not be followed by a whitespace character.
2. The end delimeter must not follow a whitespace.
3. To include a delimeter character it must be escaped with \.

### Bold

Bold begins with \* and ends with \*.
```
*This is bold*
* this is not *
```

### Italic

Begins with \_ and ends with \_.
```
_This is italic_
_ This is not _
```

### Bold-Italic

Begins with \*\_ and ends with \_\*.
```
*_This is bold-italic_*
*_ This is not _*
_* This is also not *_
```

###  Inline-Code
Begins with { and ends with }.
```
{valid}
{ not valid }
```

## Pre Block

Begins with {{{ on its own line and ends with }}} on its own line.
```
{{{
	this is
 preformatted.
}}}
```

## Keywords

The format is KEYWORD: followed by a space then the rest of the text.
```
NOTE: This is a note.
TODO: This is a todo.
WARN: This is a warning
```

## Comments

Comments begin with a # and continue to the end of the line.
```
# This is a comment.
some text here. # this is also a comment.
```

## Why?

Everyone should reinvent the wheel at least once.
