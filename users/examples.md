---
layout: default
---
# Examples

## Contents

- Examples
  - [Introduction](#introduction)
  - [Values](#values)
    - [Real](#real)
    - [Option](#option)




## Introduction

In this document we will go into details of the various types used during the Specify stage of Model creation.


## Values

A Value is the most basic of types within the project.  
You can create Values using the **M-Value** command, or as required, from within other objects.  
There are a variety of Value types that are explored more below.  


### Real

A Real value represents a real number to represent length arguments.  
There are Real Values and there are Real Objects, both of which return a value that can be used within other objects, such as Points and Vectors to represent coordinates or distances.  
Within a dialog box, there is a text field to enter the desired value.  
Alternatively there are options on the RHS for additional ways to enter a value.  


{% include note.html content="These examples are only testing functionality at the moment." %}

{% include examples.html id=site.data.examples.szlpreal %}


### Option

An Option is a value limited to a range of values, available to that type.  
An example are the Boolean values of True and False. The only possible values for that type.  
Within a dialog box, an Option is specified by selecting one of the options from the drop-down list for the value.  
The visible value is the current value.  


{% include note.html content="These examples are only testing functionality at the moment." %}

{% include examples.html id=site.data.examples.option %}


