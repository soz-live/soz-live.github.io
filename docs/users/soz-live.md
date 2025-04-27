---
layout: default

real_examples:
  - title: Basic
    text: "With a leading 0"
    image: /assets/images/favicon.png    
    alt: Test Alt Text
  - title: Intermediate
    text: "Using a Lisp Equation"
    image: /assets/images/favicon.png    
    alt: Using a Lisp Equation
  - title: Advanced
    text: "Creating a complex equation"
    image: /assets/images/favicon.png    
    alt: Creating a complex equation        


---
# SOZ-LIVE - Users

## Contents

- SOZ-LIVE - Users
  - [Introduction](#introduction)
  - [Values](#values)
    - [Real](#real)




## Introduction

**SOZ-LIVE** is a collection of over 2500 Lisp routines, that enables the creation of complex CAD entities, from a series of inputs of simpler objects.

**SOZ** interactions can be through a dialog box driven Graphical User Interface (GUI), on the command-line (CLI) or though **LIVE** a node-based UI written in **SOZ**, that enables users to create visual scripts for iterative design.

In this document we will go into details of the various types of classes and how to create them within **SOZ-LIVE**.


## Values

A Value is the most basic of types within the project.  
There are a variety of Value types that are explored more below.  



### Real

A Real value represents a real number.  
There are Real Values and then there are Real Objects, both of which return a value that can be used within other objects, such as Points and Vectors to represent coordinates and length arguments.  
When entering a real into a dialog a leading 0 is required for decimal values, such as `0.24`,  and the value can also be a lisp calculation such as `(/ 1.0 3.0)` and the resultant will be calculated as required.

Other examples of Reals, are below.

{% include examples.html id=page.real_examples %}

Date: 20250427.1021
