# Regex Tutorial

## Introduction
 Regex, short for regular expression, is a powerful tool used for pattern matching and manipulating text. It provides a concise and flexible way to search, match, and replace strings based on specific patterns.

## Summary

A regular expression is a sequence of characters that defines a search pattern. It consists of regular characters (e.g., letters and digits) and special characters called metacharacters that define the rules for pattern matching.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

Email matching regex

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

### Anchors
The anchor is what starts and ends the regular expression. The ^ is the start anchor and the $ is the end anchor. The ^ anchor is used to match the beginning of a string and the $ anchor is used to match the end of a string.

A regex is also considered a literal so it must be wrapped in `/`.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


The anchors are the ^ and the $. This code specifically is saying that we are looking for something that starts with
 `^([a-z0-9_\.-+]+)` , and ends with `([a-z\.]{2,6})$`.



### Quantifiers
A quantifier is used to determine how many times a specific character needs to be present in order to match. 

If we use the code form our regex `^([a-z0-9_\.-+]+)`, this will match any string a-z, 0-9, _, ., or -. The quantifier is the `+` and means that it has to contain at least one of these on order to match.



### OR Operator
The OR operator  is not used in our email regex example. but the following regex does. 

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

An OR operator starts with `#`.

`/^#?([a-f0-9]{6}` will match a character that is a-f or 0-9 and has to be 6 characters long.

`|` IS THE OR operator.

`[a-f0-9]{3})$/` will match a character that is a-f or 0-9 and has to be 3 characters long.

So the following regex `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` will match a string that starts with `#` and is followed by either 6 characters that are a-f or 0-9 or 3 characters that are a-f or 0-9.

### Character Classes

In a regex character classes are used to match only one out of several characters. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The `\d` is present the the email code saying that it must match an a-z character after the `@`, and not a special character or number.

### Flags

A regex Flag is not used within our email code. Regex has 6 different flags that all have a different purpose. 

i	Ignore Casing	Makes the expression search case-insensitively.
g	Global	Makes the expression search for all occurrences.
s	Dot All	Makes the wild character . match newlines as well.
m	Multiline	Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
y	Sticky	Makes the expression start its searching from the index indicated in its lastIndex property.
u	Unicode	Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

You can add a flag by using forward slashes `//`

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
