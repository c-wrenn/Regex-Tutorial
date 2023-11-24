# Matching an Email Regex Tutorial

In this lesson, I will walk through the use of one of the more popular Regular Expressions and clarify several key regex ideas by explaining how it operates.

## Summary

This is a Regex tutorial for matching an Email. We will breakdown the following regex, explaining what each component does.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

The anchors ^ and $, are used in the regex code for matching an email. A string that starts with the characters that come after it is indicated by the ^ anchor. A string that finishes with the characters that came before it is indicated by the $ anchor. It can be preceded by a precise string or a range of potential matches, much like with the ^ character.

### Quantifiers

Quantifiers define the bounds of the string (or a substring of the string) that your regex matches. Often, they contain the minimum and maximum character count that your regex is searching for. A quantifier used in this regex is  {2,6} which will allow a match range of 2-6 characters for the character set of [a-z\.].

### Character Classes

In a regex, a character class specifies a collection of characters that can appear in an input string to satisfy a match. This regex uses the \d character class. This character class matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

### Grouping and Capturing

We will utilize three capturing groups in this regex tutorial. The first capturing group, 
([a-z0-9_\.-]+), matches the users email name. The second group, ([\da-z\.-]+), will match the email service. The last capturing group, ([a-z\.]{2,6}), will match the .com.

### Bracket Expressions

A bracket expression is an expression enclosed in square brackets. Anything inside of the 
the regex code for matching an email utilizes the character sets [a-z0-9_\.-], [\da-z\.-], and [a-z\.]. The bracket expression [a-z0-9_\.-] will match any string that contains the letters a-z and is case sensitive. It will also match any number 0-9 and the characters '_' and '-'. The next bracket expression [\da-z\.-] matches  a single digit from 0-9, any character a-z (case senstive), and the characters "-" and ".". Our last bracket expression, [a-z\.], matches any character a-z, is case sensitive, and matches the character ".".

### Greedy and Lazy Match 

This regex uses two greedy matches. The quantitifier + matches the pattern one or more times. The {} quantifier matches the pattern at least two times. 

## Author
Crislyn Wren is a software developer living in Dallas, Texas.
Github: https://github.com/c-wrenn
