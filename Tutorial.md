# How Regex does Password Validation

## Summary
In this tutorial, I'll break down a regular exression (regex) used for password validatins. This regex makes sure that the password is strong and secure by checking for length, uppercase and lowercase letters,digits and special characters.

The regex pattern we will break down in this tutorial is:
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
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
The regex begins with ^ and ends with $. these are known as anchors:

The ^ anchor is used to assert the position at the start of a string

The $ anchor is used to assert the position at the end of a string

EXAMPLES
Matches: Password123!
Doesn't Match:  Password123!(extra space makes if fail)

### Quantifiers
The {8,} quantifer specifies that the preceding character class must occur at least 8 times 

{8,}: this makes sure that the password has at least 8 characters.

EXAMPLES:
Matches: Password1!,AbCdE123!
Doesn't Match: Sab1!

### Character Classes
The character class [A-Za-z\d@$!%*?&] defines what characters are allowed in the password.

A-Za-Z: Is used to match uppercase and lowercase letters.
/d: Is used to match any single digit.
@$!%*?&: Is used to match the specitfied special character.

This makes sure the password can only have letters, digits, and specified special characters.

EXAMPLES:
Matches: Password1!,AbCdE123!
Doesn't Match: Sab/enri1 

### Flags
Flags are optional. The are modifiers that change how the pattern is read. They can control things like case sensitivity, multiline matching and globle search.

EXAMPLES
i(ignore case):makes so the pattern is case-insensitive.
m(multiline): Treats beginning ^ and ending $ anchors as working across multiple lines in the input string.
g(global search): maskes it so it searches for all matches in the input string, not just the first.

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

