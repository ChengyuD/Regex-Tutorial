# Regex Tutorial

Regex, known as regular expression, is a search pattern formed by a serires of special charaters that includes the followings: anchors, quantifiers, grouping constructs, bracket epxressions, character classes, OR operator, flags, and character escapes.


## Summary
This regex tutorial will demo the explain the parts of regular expressions and their functionality for email matching `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`.


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
A regular expression is wrapped with (/) slash characters like the example given in summary.


### Anchors
Anchors are symbols at the beginning and end of a string:
- '^' symbol matches the beginning of the string for its position;
- '$' symbol matches the end of the string for its position.


### Quantifiers
Quantifiers is the preceding token to match a certain number of times:
- '+" symbol matches 1 or more of the preceding token;
- {2, 6} match between 2 and 6 of the preceding token;


### Grouping Constructs
Grouping is constructed by () in the expression and each set of parentheses is a single group to be treated as a single unit.

Take  an example from the email expression, within the anchors, there are three sets of parentheses:
- ([a-z0-9_\.-]+)
- ([\da-z\.-]+)
- ([a-z\.]{2,6})


### Bracket Expressions
Bracket expression represents a single charater, which mathes any character in the set:
- [a-z0-9_\.-]: the string can have only lower case characters that is between a to z,any numbers that is between 0 to 9, and a '_', '.' and '-' character;
- [\da-z\.-]: the string can have any digit character (0-9), lower case characters that is between a to z, and a '.' and '-' character;
- [a-z\.]: the string can have only lower case characters and a '.' character.


### Character Classes
Character classes defines a set of charaters of which occur in a string. Here is the character classe from the email example:
- '.' matches any character except the newline character (\n);
- '\d' matches any Arabic numberal digit. This class is equivalent to the bracket expression [0-9];
- '@' matches a "@" character.

### The OR Operator
OR operator is presented with (|), which is not presented in this tutorial,


### Flags
Flags are placed at the end of a regular expression, after the second slash, which define additional functionality or limits for the expression. 


### Character Escapes
Escapes is a regex character that is presented (\). In the email expression:
- '\.' matches a '.' character.


## Author
Written by Cheryth D and more information can be viewed at https://github.com/ChengyuD.