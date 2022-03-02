# Regex tutorial for matching a complex password 
In this special tutorial we will learn the regex for marching a complex password. We will also learn and understand how each part of the expression and what is responsible for controlling which part of the password.

## Summary
Welcome, this tutorial describes the regex sequence of characters that defines how to create a complex password. This password must be 8 characters, at least one Uppercase, Atleast one number, at least one lowercase case,and at least one special character. Regex are frequently used to validate input, as when included in code or search algorithms. I am going to show you a bunch of really cool Regex tricks and clean coding tips which will make working with Regex in JavaScript much easier.

## Table of Contents

- [Anchors](#anchors) *, {8,}
- [Quantifiers](#quantifiers) * + ? {}
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing) ()
- [Bracket Expressions](#bracket-expressions) []
- [Greedy and Lazy Match](#greedy-and-lazy-match) *
- [Look-ahead and Look-behind](#look-ahead-and-look-behind) (?= )

## Regex Components

### Anchors
Anchors match the start(*) and end{8,} of a given string.

### Quantifiers
As i stated in the anchor, the two most important quantifies needed in this tutorial is the *, which basically means it will match zero of more of the proceding representation. its allows the password to include any character sets we describe in the code and normally comes in the begibing of the character set and the next quantier is {8,}. This th ethe miminum character length we want our code to be. say for instant if we want a more than 8, lets say 12 then the character length would be {12,} 
### OR Operator

### Character Classes
The regex for this tutorial requires 4 different types of characters. We have uppercase letters, lowercase letters, specaial characters and numbers. Lower case letters can be represented in the code as [a-z]. The characters for the numbers will be [0-9]. For uppercase it can be found in the code like [A-Z]. Lastly special characters are prepresented as[!@#$%^&*()_+=-{}|:";'><,.??] 
### Flags

### Grouping and Capturing
Grouping and capturing are very important in this project because it breakes down each requirement of our password and let each characters to be stored in specific groups. example we know that our password should have at least one uppercase so it captures and group them in [A-Z]. At least we should have one lower case hence, [a-z]. At least our password should have one number hence [0-9]. At least one special character so we capture and group it in [!@#$%^&*()_+=-{}|:";'><,.??]

### Bracket Expressions
A bracket expression matches every single character or combination of characters within the character set. In this case a bracket expression [] can be used to match what special character you want to use in your password. in our case bracket expressions containing range expressions are used when defining numbers, uppercase, and lowercase letters and even special characters.

### Greedy and Lazy Match
The quantifier characters * and {8,} are greedy operators which expand the match as far as possible through the string to get the right password.

### Look-ahead and Look-behind
A good lookahead is written (?= )
in our regex expression an uppercase lookahead is (?=.[A-Z]), lower case is (?=.[a-z]) and so on.
look-ahead allows you to ensure that a special character occurs at least one and that the position doesnt actually matter 

## Author
This tutorial is created by Benjamin Amakye. you can go to my ###github profile and check more about me. or via email bamakye20@gmail.com
http://github.com/sirbenji03
