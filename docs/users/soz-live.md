---
layout: default

real_examples:
  - title: Basic
    text: "With a leading 0"
    image: /assets/images/egs-real-1.png    
    alt: Test Alt Text
  - title: Intermediate
    text: "Using a Lisp Equation"
    image: /assets/images/egs-real-2.png    
    alt: Using a Lisp Equation
  - title: Advanced
    text: "Adding a list of Reals"
    image: /assets/images/egs-real-3.png    
    alt: Using the ADDS function        


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
You can create Values using the **M-Value** command, or as required, from within other objects.  
There are a variety of Value types that are explored more below.  



### Real

A Real value represents a real number.  
There are Real Values and there are Real Objects, both of which return a value that can be used within other objects, such as Points and Vectors to represent coordinates and length arguments.  

{% include examples.html id=page.real_examples %}

Date: 20250427.1201
