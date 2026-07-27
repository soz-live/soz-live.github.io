---
layout: default
---
# Value

## Contents

- Value
  - [Introduction](#introduction)
  - [Option](#option)
  - [Real](#real)
  - [SZLPReal](#szlpreal)



## Introduction

A Value is the most basic of types within the project.  
You can create a Value using the **M-Value** command, or as required, from within other objects.  
There are a variety of Value types that are explored more below.  

> Notes:  
> - It is possible to utilise the Key of another Object as the value if the Type is suitable.  
> - It is also possible to select a Method which returns the same type as that required.  


## Option

An Option is a value limited to a range of values, available to that type.  
An example are the Boolean values of True and False. The only possible values for that type.  
Within a dialog box, an Option is specified by selecting one of the options from the drop-down list for the value.  
The visible value is the current value.  


## Real

A Real value represents a real number to represent length arguments, etc..  
There are Real Values and there are Real Objects, both of which return a value that can be used within other objects, such as a Point or a Vector to represent coordinates or distances.  
Within a dialog box, there is a text field to enter the desired value.  
Alternatively there are options on the RHS for additional ways to enter a value.  


## SZLPReal

A SZLPReal Object represents a Real number as an Object. And is passed and returned as an ID.  

Subclasses of SZLPReal include means to create mathematical equations such as:

- +: Addition
  - SZLP-ADD to add two numbers and 
  - SZLP-ADDS to add a list of values
- -: Subtraction
  - SZLP-SUB to add subtract numbers and 
  - SZLP-SUBS to subtract a list of values
- \*: Multiply
  - SZLP-MUL to muptiply two numbers and 
  - SZLP-MULS to muptiply a list of values
- \/: Divide
  - SZLP-DIV to divide two numbers and 
  - SZLP-DIVS to divide a list of values
  

