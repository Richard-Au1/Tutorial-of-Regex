# Using RegEx to Batch File renaming

Regex allows users to save plenty of time when doing text processing through a file or any other informational system.

## Summary
Regex can be used to alter text on a file with less time spent doing so. Using the characters that regex comprised of `(/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/)`, we can save time while updating, creating, deleting, or searching for information within a file. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)

## Regex Components

### Anchors
Anchors will mark the beginning and end of an expression. As ^ marks the beginning of the expression and $ will mark the end of an expresssion such as `/^[0-9]/` and `/t$/`. This can be used when searching for expression that contains certain characters in a file to update them to be the same. 

### Quantifiers
Quantifiers is used after an expression to show how many times it can be repeated. For example, if `?` is used then the character used should only be repeating in a row once. While if `*` is used then it can be repeated infinitely.

### Grouping Constructs
Grouping constructs can be used to signify a group of characters within a certain parameter such as `(/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/)`. The symbol for grouping is `()`. This is the first part of the set of constructs ([a-z0-9_\.-]+)@([\da-z\.-]+), and secondly ([a-z\.]{2,6})$/). The first part allows two different sets of parameters to be met with using this grouping. While the second set of parameters only wants that specific set of characters to match.

### Bracket Expressions
Similar to the grouping construct, Bracket expressions allows the system to search for the selected information within the brackets. For example, if `[0-9]` is the expression in which is being stated then the file will allow search within the file to find the instance of the characters in the bracket. Allowing the user an easier time to search through the file to update or delete information with the file.

### Character Classes
Character classes help distingush characters from one another such as letters and digits.  For example, `\d` refers to digits or numbers and `\w` matches expressions in the alphanumerical characters. Similar to Bracket expressions, these can be used to search for phrase within a document instead of reading throughout the document to find the each instance that is being specified in the search field. 

### Flags
Flags are similar for searching through the document as Bracket expressions because they search specific regex expression depending on the command used. For example, g looks through the entire global search and i does a case sensitive search. How the expression can look like is `const re = new RegExp("\\w+\\s", "g");`.

## Author

Hello, my name is Richard Au. I got interested in computer programming back in 2014, but I recently decided to pursue computer programming after trying other career paths. I wanted to know if computer programming was a career that I would have a passion for the rest of my life. I enjoy solving problems and getting to know to get a device operational. Here is a link to a list of apps I have created: https://github.com/Richard-Au1?tab=repositories 