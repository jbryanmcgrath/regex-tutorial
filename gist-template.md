# Regular Expression Tutorial

This is a simple tutorial to illustrate what regular expresions are and how to use them

## Summary

The snippet provided is a common regex used to identify a matcing email through pattern recognition. Other examples may be provided.

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

    Anchors are used to signify the beginning or end of a string. Common anchor are the ^(caret) or the $(dollar)

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Quantifiers

    Quantifiers are there to specify the amount of instances of a character or group.
    Common quantifiers are {n} n being a number. ?:matches 0 to 1 + matches 1 or more.

    notice the third grouping in the given example.


    ([a-z\.]{2,6})

### OR Operator

    The OR operator is simple and similar to javascript syntax. | known as (pipe).
    you could search for words that have 1 letter of difference between the Us and the Aus word.

### Character Classes

    A character class matches a character from a certain set of characters. For instance [0-9] will match with any digits 0 through 9. Another example would be [a-z], this will match any lowercase letter a through z. In the email example /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ you can see where it is looking for letters a-z, and digits 0-9.

### Flags

    Flags are added at the end of expressions. There are 3 main ones. i, g, m depending on the scope of the search.

### Grouping and Capturing

    This regex matches any letter or number a-z or 0 to 9, accepts underscores, periods and dashes. Then the quantifier matches one or more of the previous token.

### Bracket Expressions

    Bracket expressions are the syntax to combine character classes. Differeant character classes may be combined in a single bracket expression.

    Example: [a-z0-9]

### Greedy and Lazy Match

    {b,} = LAzy matches search the number in the first spot and more.
    {a,b} = greedy match that searche sin between the characters a,b

### Boundaries

/b will match positions where one side is a word, and the other is nont a word.

### Back-references

    Back-references match the same text as previously matched by capturing a group.
    ([a-c])x\1x\1

### Look-ahead and Look-behind

    This allows you to look ahead or behind in a certain expression to find the desired results.

## Author

To see more of Bryan McGrath's work, please visit the link to the github profile (jbryancmgrath)
