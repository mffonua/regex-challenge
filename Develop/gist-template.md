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
- [Grouping and Capturing](#grouping-and-capturing)
- [In Conclusion](#In-Conclusion)



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
 Our regex has one big group `([a-f0-9]{6}|[a-f0-9]{3})` which is divided by an OR Operator `|`. Which means that in our group we have 2 expressions, `([a-f0-9]{6}` and 
 `[a-f0-9]{3})`. This means that our regex will match any of the two expressions. <br>
Ex. an OR operator using to validate zip codes, `(801|104|102)` will match those "801","104" or "102" as part of a zip code.
### Character Classes
In our regex we have one character class that is repeated twice: `[a-f0-9]`. A character class matches any character enclosed in brackets. For example: `[abc]` will match "a" or "b" or "c". `[-.]` will match "-" or ".". 

Inside our character class we have two ranges: `a-f` and `0-9`. This means that it maches any character "a" through "f" (lowercase, it won't match uppercase), and "0" through "9".  Other examples: `[m-p]` matches "m", "n", "o" or "p". `[3-5]` matches "3", "4" or "5".

### Grouping and Capturing
This Regex ExExpression has one group, and it is used in combination with the OR Operator (as listed above).

### In Conclusion
After analyzing every part of our regex `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`, we could describe its matching patern like this:

"Every sequence of characters that starts with # or not, followed by 6 charcaters "a" through "f" and "0" through "9", OR followed by 3 charcaters "a" through "f" and "0" through "9"."
## Author

Hello, My name is Miles Fonua, I am a full stack developer student looking to learn and grow. I want to focus more on front end development (as I find it more visually appealing) however I will still work on back-end dev. work as well. If you have any questions or suggestions please reach out to me via [LinkedIn](https://www.linkedin.com/in/miles-fonua-24b791237/) or Email @ <a href="mailto:myles.fonua@gmail.com">myles.fonua@gmail.com</a>.

GitHub: [mffonua](https://github.com/mffonua)