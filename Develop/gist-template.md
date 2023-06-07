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

### Anchors
The anchor is what starts and ends the regular expression. The ^ is the start anchor and the $ is the end anchor. The ^ anchor is used to match the beginning of a string and the $ anchor is used to match the end of a string.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The anchors are the ^ and the $.This code specifically is saying that we are looking for something that starts with `/^([a-z0-9_\.-]+)`.

We will define what everything else inside the parenthesis means in the next section, but the anchor is the first thing we see.

### Quantifiers
A quantifier is a metacharacter that specifies how many instances of a character, group, or character class must be present in the input for a match to be found. The most common quantifiers are` ?,`` *,` and` +`. For our code the regex `xyz+` matches the string` xyz` followed by one or more `z` characters.

`([a-z0-9_\.-]+)`

This will match any string that contains `a-z, 0-9, _, .,` or `-.` The quantifier is the +. This code specifically is saying that we are looking for something that starts with 

`/^([a-z0-9_\.-]+).

This will match any string that contains `a-z, 0-9, _, .,` or `-.` The quantifier is the `+` means that it has to have at least one of the characters in the brackets. The `+` is the quantifier.


### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
