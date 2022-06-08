# Regex Tutorial

This is a tutorial designed to teach certain basic concepts of regex. Regex is short for regular expression, which is a string of text that allows one to create search patterns that help match, locate and manage text inside a body of text.  

## Summary

This tutorial uses the following regex, which matches email addresses, as an example of the concepts discussed below:  

/^([a-z0-9_\\.-]+)@([\da-z\\.-]+)\.([a-z\\.]{2,6})$/

Specifically, this tutorial covers:  

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

Anchors are tokens that do not match a character in a body of text but instead modify the characters before or after the token by requiring the otherwise matching characters to occur at a particular a position within the string being searched.   For example, "^" requires the otherwising matching character to occur at the beginning of a text line and "$" requires them to occur at the end of a string.  

From our example, ^([a-z0-9_\\.-]+), the "^" anchor requires a match to the character class to occur at the start of the email.  Similarly, the "$" in ([a-z\\.]{2,6})$ requires the match that satisfies the shown character class with the shown quantifier to occur at the end of the email.  



### Quantifiers

Quantifiers are meta characters that modify the previous characters in a regular expression by quantifing how many times the preceding character(s)in the regular expression should be repeated.  

In this part of our example, [a-z0-9_\\.-]+, the "+" is the quantifer that requires 1 or more matches of the preceding character class (see below for explanation of character classes).  

Another example of a quantifier is in this part of the example, [a-z\\.]{2,6}.  Here, the "{2,6}" is a quantifier which follows the  pattern of {min matches, max matches}.   In our case, this means that there needs to be between 2-6 matches of the preceding character class.  
### OR Operator

### Character Classes

Character classes allow matching only one out of several characters in a set.  The set of characters that can be matched are placed between square brackets.  

In our regex example, [a-z0-9_\\.-] is a character class which is satisfied by either a lower case letter between "a-z", a digit between "0-9", an underscore, a period or a dash.  

[\\da-z\\.-] is another character class in the example that is satisfied by any digit (which is designated by "\d"), a lowercase letter between a-z, a period or a dash.

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
