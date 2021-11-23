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

The OR operator, |, is used to match characters of either the left or the right of the | operator.

### Character Classes

A character class allows you to match any symbol from a certain character set such as \d which turns a phone number with special characters such as (, ), and - into a plain text number.

### Flags

Flags are tokens that modify its behavior of searching. 
The i flag makes the expression search case-insensitively.
g makes the expression search for all occurences.

### Grouping and Capturing

Grouping and capturing expresssions are a way to treat multiple characters as a single unit.
((A)(B(C)))

### Bracket Expressions

A bracket expression is either a matching list expression or a non-matching list expression.
[:alnum:] is also the same as [0-9a-zA-3]

### Greedy and Lazy Match

A greedy match matches the longest possible string while a lazy match matches the shortest possible string.

### Boundaries

A word boundary is a postion between /w and /W (non-word character), or at the beginning or end of a string.

### Back-references

A backreference identifies a previously matched group and looks for exactly the same text again.
@"(\b\S+)\s+\1\b"

### Look-ahead and Look-behind

Lookahead asserts that what immediately follows the current position is an uppercase letter.
Lookbehind asserts that what immediately precedes the current position is a lowercase letter.
Lookahead (?=foo)
Lookbehind (?<=foo)

## Author

Anthony Her is was raised in Hickory, NC and graduated with a Bachelor's of Science in Biology. He has worked in many labs and now is looking for a career change into the tech world.

GitHub: https://github.com/antpher