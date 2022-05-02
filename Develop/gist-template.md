# REGular EXpressions (REGEX) Made Simple

This tutorial will break down a regular expression and explain the different components piece by piece. In general, they are used to define search queries within any string of text by means of notation specific to them and enclosed within '/' or back slash characters.

## Summary

The following regular expression is used to locate a valid email address.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

/`^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`$`/

Anchors, denoted by `^` at the beginning and `$` at the end, mark the boundaries of a Regex expression in conjunction with the `/` characters. They allow a search function to know where the expression starts and ends.

### Quantifiers

/^([a-z0-9_\.-]`+`)@([\da-z\.-]`+`)\.([a-z\.]`{2,6}`)$/

Quantifiers, denoted in this example by `+` and the curl brackets `{ }` specify how many instances an expression occurs. The `+` indicates that the expression within the curl brackets should occur one or more times to register on the search function. The `{2,6}` indicates that the expression should occur between two and six times, including twice and six times.

### Grouping Constructs

/^`(`[a-z0-9_\.-]+`)`@`(`[\da-z\.-]+`)`\.`(`[a-z\.]{2,6}`)`$/

Grouping constructs, such as the parentheses `()`, separate expressions when searching for expressions that occur at different frequencies or are separated by other characters such as the `@` symbol.

### Bracket Expressions

/^(`[`a-z0-9_\.-`]`+)@(`[`\da-z\.-`]`+)\.(`[`a-z\.`]`{2,6})$/

Bracket expressions, indicated by `[ ]`, indicate an individual character in a search. Multiple character types can be enclosed within the brackets sequentially to indicate "or" within the confines of the expression. For instance, on the first expression `[a-z0-9_\.-]`, it indicates to search for an alphabetical character `a-z`, a numeric character `0-9`, an underscore `_`, a period `\.`, or a hyphen `-`.

### Character Classes

/^([`a-z` `0-9``_`\.`-`]+)`@`([\da-z\.-]+)\.([a-z\.]{2,6})$/

Character classes are the types of characters that are contained in the expression and that regex looks for. The specific character types in this example are indicated in the Bracket Expressions section immediately above.

## Author

Jonathan Nguy

I am a software programmer who lives to learn about life. My goal is to create my own game applications.

GitHub: https://github.com/alraune-belladonna
