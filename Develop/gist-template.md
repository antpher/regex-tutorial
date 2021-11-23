# RegEx Tutorial

In this tutorial, I will explain explain regular expressions, or regex for shot, by deconstructing the expressions and explaining what each part means.

## Summary

Below is a regex expression to match a hex value.

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The / indicates the start of a regular expression
^ matches the beginning of the string
The # matches a # character
? matches between 0 and 1 of the preceding token
( captures group 1
a-f is the range of letters allowed (case sensistive)
0-9 allows numbers 0-9
{6} matches 6 of the preceding tokens
{3} matches 3 of the preceding tokens
$ indicates the end of the string
Closing / indicates the end of the expression


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

Anchors do not match characters, but instead they match a position before or after characters.

The ^ anchor matches the beginning of the text and the $ matches the end of the text.

### Quantifiers

Quantifiers specify how many instances of a character or group must be present for a match to be found such as *, +, and ?.

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
