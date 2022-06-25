# What is Regex about?

Regex is a shorthand notation that stands for regular expression.
It is a special text string used by developers to describe a search pattern
when included in coding or algorithms. It typically is used when one is trying
to match a certain character combination within a string. Which is very helpful for pulling out information from the body that is needed in our code. This tutorial will help you understand regex and how to use it!

## Summary

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The following code above is an example of how the components within a regex can be used.
In this case, it will be used for matching emails. The components within this regex will be used to validate that an email is correctly formatted by having the necessary components of an email. 

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

What are anchors? Anchors are components within a regex that begins the regular expression and ends the expression. Take for example the matching email regex below:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Notice that the anchors in this regex are the '^' and the '$'. By breaking it down only in just the beggining portion and the end portion. This regex is searching for something that starts with ^([a-z0-9_\.-]+) this component and must end with this ([a-z\.]{2,6})$ component. For now just remember that the start of a regex beings with '^' and ends with '$'. We will discuss more about the certain components in between the anchors further in depth in this tutorial. 

### Quantifiers

What is a quantifier? A quantifier in a regex is a component used to determine how many times a certain characters or even groups of characters need to be included or present in order for it to be counted as a valid regex. A quantifier is recoginized as a '+'. Using our regex from earlier, ([a-z0-9_\.-]+), this is an example of a group of characters using a quantifier. Notice how a-z,0-9, _ , . , and - are used for this grouping. It is considered a grouping as these characters are bounded within '()'. The quantifer is basically stating that at least one of these characters have to be included in the beggining portion of this regex to be counted as a valid expression. 

### OR Operator

What is a OR Operator? A OR Operator is defined within a regex by a ' | '. It allows for a logical operator. In this case for matching an email we do not use a OR Operator. However if we were to take a look at this code below: 

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

This is an example of a Hex value and the OR Operator is being used therefore it means that the expression logic wants the search to find either hex codes that are 6 or 3 letters or digits. 

### Character Classes

Character classes distinguishes the different kinds of characters. For example, it can be used to distinguish between letters and digits. In our email regex the '\d' is the character class used. Since 'a-z' follows '\d' it represents that following an '@' in our email the next character has to be a letter. It can not be a special symbol or a digit otherwise it will not satisfy the regex. 

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
