# Regex Anchor Tutorial

Welcome! In this tutorial I will be going over one facet of regular expression: anchors.

## Table of Contents

- [What are anchors?](#what-are-anchors)
- [Beginning](#beginning)
- [End](#end)
- [Boundaries](#boundaries)
- [Word Boundary Expressions](#word-boundary-expressions)
- [Not Word Boundary Expressions](#not-word-boundary-expressions)

## What are anchors?

- Rather than matching characters as is common in regular expression, anchors match locations. Examples would be positions before, after or between characters.

### Beginning

- Let's say we have the following sentence:

      "hi how are you?"

- You can check to see if the beginning word (hi) matches with the following expression:

        ^\w+

- In this expression, you are using the regex for beginning: ^
- And the expression for word: \w
- Along with a quantifier: +

### End

- Using the previous example of:

        "hi how are you?"

- We would simply substitute the ^ with a $ like this:

       \w+$

- Moving the different character to the end, this would allow us to match with the word "you"

## Boundaries

There are a few positions that qualify as word boundaries in regex:

- Before the first character in the string, if the first character is a word character
- After the last character in the string, if the last character is a word character
- Between two characters in the string where one is a word character and the other is not

### Word Boundary Expressions

-If we continue to use the same sentence:

        "hi how are you?"

-You could match the position of the "e" in the word "are" by using the following:

        e\b

- The expression being:

        \b

### Not Word Boundary Expressions

-If you want to match something inside of the string (not boundary) you can use the following:

        \B

## Author

Hi, my name is Jordan and I'm a full stack web developer. Feel free to peruse my Github repos here:

[jorddo](https://github.com/jorddo)
