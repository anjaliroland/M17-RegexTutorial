# Regex Tutorial: Matching a Hex Value

This is a regex tutorial intended to help understand how to match a hex value with regular expressions. 

## Summary

Hex values are commonly used in programming and web development to represent colors, unique identifiers, and other data. Understanding how to match and extract hex values using regular expressions is a valuable skill for working with text data.

To start here is a regular is expression used for matching Hex Values:
`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components

### Anchors
Anchors are used to specify the position of the match within the string. In the context of matching a hex value, we use the `^` anchor at the start and the `$` anchor at the end to ensure the pattern matches the entire string.

### Quantifiers
Quantifiers define the number of occurrences of a character or group. For matching a hex value, we use `{6}` to indicate that there should be exactly six occurrences of the preceding character class.

### OR Operator
The OR operator (`|`) allows us to match alternative patterns. In the hex value regular expression, we use the OR operator to match either a six-character pattern or a three-character pattern, representing the hex triplet and shorthand hex formats.

### Character Classes
Character classes specify a set of characters that can match at a particular position in the regular expression. In the hex value regex, the character class `[a-f0-9]` represents valid hexadecimal characters (0-9, a-f, A-F).

### Bracket Expressions
Bracket expressions are used to group characters together and specify a range of characters within a character class. In the hex value regex, we enclose the character class within brackets to create a bracket expression.

### Greedy and Lazy Match
The `?` quantifier is used for lazy matching, which matches as few occurrences as possible. In our hex value regex, the `?` quantifier after the `#` indicates that the character is optional.


## Author

Anjali Roland - web dev newbie
GitHub: https://github.com/anjaliroland