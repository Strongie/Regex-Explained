# Matching a Hex Value

The following commentary will be explaining the hexadecimal regular express (otherwise known as the hex regex). 

## Summary

We are going to at a regex that will match any hexademical code in a string of characters. A string of characters know as a regular expression, designates a text search pattern. The characters in question could be literal or meta characters. Meta characters, which stand in for a larger variety or characters, are frequently used to build regex.

We will look at the following regex.

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/


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

In this specific instance, our regex uses the position meta characters $ and ^ as the two anchors. The ^ symbol denotes the beginning of a string or a line. The $ symbol denotes the end of a string or line. As an ilustration, ^abc matches any line or string that starts with the letter abc, while xyz$ matches any line or string that finishes with the letters xyz.

### Quantifiers

When determining how many times a component of your regular expression should be repeated, quantifiers are employed. You can add a quantifier to every item you want to repeat in a regex, whether it's a character, a character class, or a subexpression, to indicate how many times it should be repeated.

The hex regex uses two types of quantifiers: ? and {n}.

The quantifier ? matches any character that comes before it 0 or 1 times. The ? now functions as a kind of conditional inside the regex. Since # comes before ? in our regex, either string that starts with # or not will match our expression.

The second quantifier in our regex, {n} is utilised twice in the numbers {6} and {3}. This meta character perfectly matches the character that comes before it n times. For instance, the regular expression {\d{4}} will match any string containing four consecutive digits, such as 1234 or 7777.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
