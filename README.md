# Regex tutorial to match Email

Hello World! Using regex to verify Emails is extremely common in web development, learning to verify Emails is extremely important.

## Summary

The regex code that will be analyzed is: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,12})$/`. This may look very confusing, but we can get through this!

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

Containing the regex is done by using the `^` and `$` symbols.

### Quantifiers

In the above expression, `+` was used to say that there is another sequence to be matched. This is a 'greedy quantifier'. The numbers 2 and 12 were used at `{2,12}` to specify that there should be no fewer than 2 characters and no more than 12 in the input.

### Character Classes

`\d` is used to classify all numbers

### Grouping and Capturing

Three groups are captured in the above example. The first group is the beginning of the email (before the @) `[a-z0-9_\.-]`. The second group captures an e-mail service that is used (such as gmail, yahoo, etc.) `[\da-z\.-]`. The last group captures the extension (such as '.com' or '.net') `[a-z\.]{2,12}`.

### Bracket Expressions

Three bracket expressions are used. The info in the expressions are opened and closed by `[]`. These different expressions identify which information should be matched.

1: `[a-z0-9_\.-]` - This includes all characters from a-z (upper and lowercase), numbers from 0-9, an underscore, periods, and hyphens.

2: `[\da-z\.-]` - This includes all digits, all characters from a-z (upper and lowercase), periods, and hyphens

3: `[a-z\.]` - This includes all characters from a-z (upper and lowercase), and periods.

### Greedy and Lazy Match

In the above example greedy quantifiers were the only ones used, this means that it will allow the match to expand as long as it needs to go. No lazy matches were used.

## Author

Bailey Poe

GitHub Repository: [Click Here](https://github.com/bpoe1222)
