# Matching an Email Tutorial

In this document I will be creating a tutorial to explaining how the regex for matching an email functions as well as breaking down and describing each part of the expression.

## Summary

A regex or formally known as a regular expression, is a series of characters that defines a search pattern. This tutorial is going to explain the use of a regualar expression to match an email using the expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors

In a regular expression for matching an email uses the anchor ^. This shows the beginning of a string. The ending of a string is indicated by $. 

### Quantifiers

This regex contains the following quantifiers. {2-6} allows a range of 2-6 characters for the character set of [a-z\.], the + operator connects the email name + .com. 


### Character Classes

This regular exprssion uses the character class \d, this matches a character that is a single digit from 0-9. For example it would be able to match '2', and not '22'.


### Grouping and Capturing

The first capturing group in this regualer exprssion matches the users email name, ex: ([a-z0-9_\.-]+). The second matches the email service used, ex: ([\da-z\.-]+). The 3rd and final capturing group will capture .com, ex: ([a-z\.]{2,6}).  

### Bracket Expressions

 There are three bracket expressions within this regex:

[a-z0-9_.-], [\da-z.-], and [a-z.]

[a-z0-9_.-] this matches any charater 0-9 or any letter a-z, as well as ('_', '-', '.').

[\da-z.-] this matches single digits 0-9, any letter(case sensitive) and ('_', '-')

[a-z.] this matches the character ('.'), and any character a-z(case sensitive)


### Greedy and Lazy Match

The regular expression for matching an email includes greedy matches since it utilizes the + Quantifier. This regex contains another greedy quantifier {}, this used when matching `{2,6}.

## Author

My name is cam and I am a new developer learning to code and have fun along the way. If you want to view any of my work visit my GitHub: https://github.com/camkaras
