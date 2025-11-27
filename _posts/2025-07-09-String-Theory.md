---
layout: post
author: Tim_M
---

We live in a world where we interact through strings, via languages, whether they be human, written, spoken, computer or mathematical.

## Strings

Strings are human-readable code for ideas, concepts, classes and descriptions.  
They are written in the language of choice and can be converted between different languages to suit the end-user.

## Symbols

Symbols are human understandable, computer-readable code for ideas, concepts, classes and descriptions.  
Together with syntax, symbols make up part of a programming language.
Within **SOZ** symbols are used that shadow strings within the code for function arguments and object properties.

## Numbers

Numbers are human understandable, mathematical-readable code for ideas, concepts and equations.  
When we talk about numbers - we are translating strings into numbers for use within mathematical constructs such as equations and geometric functions.
And as with a programming language, there are other symbols and syntax that are used to convey the meaning.

## Conclusion

**SOZ** uses strings in places where other programming languages might use symbols, because:

- Users have to be able to read the strings.
- converting strings to symbols is easy.
- It enables automatic documentation of the system.

**SOZ** then uses routines to convert strings into the language required.

- String -> Symbol for within Lisp.
- String -> Number for within equations.

It makes perfect sense then to use Strings as the basis for human understanding and communication as well as for conversion into other forms for the various purposes as required.