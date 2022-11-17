# Regex Matching A Hex Value
Regular Expressions (Regex) are a sequence of characters that specifies a search pattern in text.
The Hexadeximal (Hex) is a postional numeral system that uses 16 distinct symbols. 

One of the uses of the Hex system are the hex color codes (a hexadecimal representation of a color in RGB format.)
Examples of the Hex Color Codes are : <br>
`#4169e1`
`#6d6771`
`#FFFDD0` 


## Summary

We are going to analyze a Regular Expression or [Regex](https://en.wikipedia.org/wiki/Regular_expression) that matches any hexadecimal code in a string of characters. <br>
The regex that we are going to analyze today is: <br>
`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

This Regex will allow us to find any hex code.


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
The anchors for this string are `^` and `$`.

The `^` meta character represents the beginning of the string and the `$` represents the end of the string. 
For example, `^xyz` wont match any string that begins with xyz, and `abc$` wont match any string that ends with abc. Our regex uses `^` and `$` to make sure that we are matching the full expression `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` from the beginning to the end.

### Quantifiers
This regex uses 2 types of quantifiers `?` and `{x}`.
`?` matches any proceeding character 0 or 1 time. This makes the `?` a conditional inside regex. Since `#` is preceeded before the `?`, our expression will match a string that either begins with a `#` or not. <br>
Ex. `\th3?r` would match both "their" and "there".
The other quantifier that is used in our regex is `{x}`, it is used 2 times ( `{6}` and `{3}` ). This matches exactly the preceding character x-amount-of-times. <br>
Ex. `{\d{7}}` this regex will match any string that has 7 consecutive numbers like `1234567` or `8410411`.
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

Hello, My name is Miles Fonua, I am a full stack developer student looking to learn and grow. I want to focus more on front end development (as I find it more visually appealing) however I will still work on back-end dev. work as well. If you have any questions or suggestions please reach out to me via [LinkedIn](https://www.linkedin.com/in/miles-fonua-24b791237/) or Email @ <a href="mailto:myles.fonua@gmail.com">myles.fonua@gmail.com</a>.

GitHub: [mffonua](https://github.com/mffonua)