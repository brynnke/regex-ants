# Regex Toutorial on  matching email

Regular expression aka regex, is a simple pattern of characters. These characters are used to search and find patterns in strings. They also find and replace characters within a string or validate input. 


## Summary
This tutorial is going to explain the use of regex to match emails using: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 
The regex we are analyzing matches character information for valid e-mail addresses. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors

Anchors used to contain this regular expression include: ^ (to start), and $ (to finish). 

### Quantifiers
Quantifiers are used to lay out how many times given characters are expected to appear. 
The + is a quantifier. This quantifier will connect the email-name and email carrier and .com. {2,6}, is a quantifier as well, this will allow a match range of those alloted numbers. 


### Character Classes
Character class in the above expression is \d. \d matches a single character, that is a digit from 0/9. It only matches to single digits, no doubles. 

### Flags

### Grouping and Capturing

The first capturing group is ( [a-z0-9_\.-]+). This matches user emailname. ([\da-z\.-]+), matches the email carrier. ([a-z\.]{2,6}), captures the last part of the line the .com. 

### Bracket Expressions

The included bracket expressions [a-z0-9_\.-], [\da-z.-]. The first one matches any letter and is case senstive, as well as matching charcters 0-9. It also matched characters '_,-' as well. The second expression matches any character within the parameters. 

### Greedy and Lazy Match

The email regex does include greedy matches. Because is has the + quantifier, it will match as many given times you need. Using {} is a greedy as well. 


### Boundaries

## Author
My name is Brynn. I am currently learning full-stack web development. This is my first go at a gist! 
https://github.com/brynnke

## sources
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions
