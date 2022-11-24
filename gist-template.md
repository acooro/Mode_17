# Title (replace with your title)
Regex Tutorial

## Summary

Today we will be talking about regex which is short for regular expressions. The regex I'll be talking about is

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

which is to use to valid email addresses. 

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
Basic Element
. = matches any single character

\followed by a single character = Lets special charcters be used as a single character

'$' = 	Matches any string where the specified pattern occurs at the end of the string

'^' = Matches any string where the specified pattern occurs at the beginning of the string

[ ] = Matches any single character in the range or set enclosed in the brackets

'|' = OR operator

() = Grouping expressions
### Anchors

Anchors are regex tokens that don't match any characters but help with the string or the matching process. Anchors matches a location which can be the beginning or the end of a string

### Quantifiers

Quantifiers match a number of instances of a character, group, or character class in a string

### Grouping Constructs
Grouping and capturing of users email
grouping and capturing of the service provider
grouping and capturing of the domain name

### Bracket Expressions
`/^([az09_\.-]+)
Matches any character in the square brackets
ex : [az09_\.-]

@([a-z]+)\
Matches any character in the range of characters separated by a hyphen ( - ) 
ex: [a-z]

.([^a-z\.]{2,6})$/`
Matches any character except those in the square brackets or in the range of characters separated by a hyphen ( - ). ex: [^a-c][^abcd]]



### Character Classes
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Character classes are what is define with in the []
[a-z0-9_\.-] : A to Z letters and 0-9

### The OR Operator
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The OR operator allows us to do two different results cases depend on what we need.  So if needed the email to end with .com or .net we would add (.com |.net)

### Flags
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
There are total of 6 flags for searching:
i = case-insensitive
g = matches all
m = multiline mode
s = dotail mode 
u = unicode support
y = sticky mode


### Character Escapes
\ in an expression precedes a literal character. 
\w for a word character
\s for a space


## Author

Dong Nguyen - Bootcamp student
https://github.com/acooro
