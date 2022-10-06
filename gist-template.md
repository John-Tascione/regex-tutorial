# REGEX Tutorial

The below tutorial will summarize a specific regex. The tutorial is broken into a summary section, which will discuss the regex's function wholistically, and additional sections for each component of the regex. 

## Summary

The regex which will be discussed in this tutorial is `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/` which is used for mathcing a url value. This regex will match a string which begins with https:// then includes all letters between a and z followed by a period folowwed by between 2 and 6 lowercase letters inclusive. 

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

The anchor characters signify that a string should begin or end with a certain character. The anchor characthers for a regex will either be an ^ or a $. In the url matching regex discussed in this tutorial the anchor character ^ indicates that the URL must begin with https and the $ indicates that the expression must end with  which signifies that the s
### Quantifiers
Quantifiers in a regex are signified by {}. In the above url matching regex the quantifiers {2,6} are used to define that the string of characters between a and z must have between 2 and 6 letters. 
### Grouping Constructs
Grouping constructs in a regex are identified by (). The regex will then look for a part of the string to match what is contained within the (). In our URL match regex the first grouping contruct is (https?:\/\/)?. This means that a string which matches must begin with https
### Bracket Expressions
In a regex bracket expression represesnt a range of characthers which should match. In the URL match regeex there are 3 bracket expresions. The first [\da-z\.-], signifies that this portion of the string must match either a didget between 0-9 or a lowercase letter. 
### Character Classes

### The OR Operator
The OR operator in regex is denoted as |. This will return a match as long one portion of the grouping construct is found.  This operator is not used in our URL matching regex. 
### Flags

### Character Escapes
Character escpaes in regex allow charachters to be next to eachother that would outherwise cause literal interetation. In the URL matcher the escapes are noted as \ and are used in the https: grouoping construct to allow two // to be positioned next to eachoter. 
## Author

This tutorial was written by John Tascione. Other projects from John can be found on his github profile at: https://github.com/John-Tascione
