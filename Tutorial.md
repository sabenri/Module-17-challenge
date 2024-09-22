# How Regex does Password Validation

## Summary
In this tutorial, I'll break down a regular exression (regex) used for password validatins. This regex makes sure that the password is strong and secure by checking for length, uppercase and lowercase letters,digits and special characters.

The regex pattern we will break down in this tutorial is:
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$


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
The regex begins with ^ and ends with $. these are known as anchors:

The ^ anchor is used to assert the position at the start of a string

The $ anchor is used to assert the position at the end of a string

### Quantifiers
The {8,} quantifer specifies that the preceding character class must occur at least 8 times 

{8,}: this makes sure that the password has at least 8 characters.

EXAMPLES:
Matches: Password1!,AbCdE123!
Doesn't Match:Sab1!

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

