---
layout: default
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

A Real value represents a real number to represent length arguments.  
There are Real Values and there are Real Objects, both of which return a value that can be used within other objects, such as Points and Vectors to represent coordinates.  

{% include note.html content="These examples are only testing functionality at the moment." %}

{% include examples.html id=site.data.examples.szlpreal %}

Date: 20250502.1752
