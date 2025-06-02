---
layout: default
---


# Lisp Intro

## Contents

- Lisp Intro
  - [Lisp Introduction](#lisp-introduction)
    - [Lisp Background](#lisp-background)
    - [AutoLISP Limitations](#autolisp-limitations)
    - [AutoLISP Development](#autolisp-development)
    - [AutoLISP Future](#autolisp-future)
  - [Lisp Basics](#lisp-basics)
    - [Lisp Functions](#lisp-functions)
    - [Function Renaming](#function-renaming)
  - [Types](#types)



## Lisp Introduction

Lisp, short for LISt Processing, may be one of the oldest programming languages, but it is also one of the most divisive:  

- You either like the syntax or you don't.
- You either get it's simplicity and expressiveness or you don't.

It is for some of those reasons that Lisp has been pushed to the background, with the likes of C, C++, Java, Python, Ruby and others taking the limelight. Yet, there is still a strong a thriving community of programmers who love and revere the languages that have developed from the original Lisp, including:

- Common Lisp, 
- Scheme, 
- Racket, 
- Clojure.


### Lisp Background

Since early on in the history of AutoCAD, a dialect of Lisp was included as a scripting programming language to enable users to improve productivity through the creation of scripts, routines and commands that enabled users to automate complex, repetitive and tedious tasks.
Because of these abilities, Lisp programming became popular amongst many CAD users and a thriving community of programmers pushed the limits of what the language could do.  
  
As competitors to AutoCAD came into the market, they realised the potential, importance and strengths of including the Lisp application programming interface (API) with their products and providing support for users crossing over to their products. 
Thereby enabling users to bring their collection of routines developed over the years with them and maintain their levels of productivity.


### AutoLISP Limitations

Because of its roots, AutoLISP, and it's associated Dialog Control Language (DCL), suffer from limitations when compared to other dialects of Lisp such as Common Lisp and Scheme.  
Limitations of the language include the lack of an object system, a macro system, defining functions with a variable number of arguments and the ability to create closures.
Despite that, developers continue to work on improving it by providing solutions to shortfalls in functionality. 


### AutoLISP Development

While AutoDesk added an Integrated Development Environment (IDE) and support for ActiveX objects in VisualLisp since AutoCAD 2000, there seems to be little interest to improve the AutoLISP API beyond VisualLisp.  
Bricssys, the developer of BricsCAD, has arguably led the way in this regard, with extensive support for Lisp functionality provided by the program as well as continued development of the API and the release of the BricsCAD Lisp Advanced Development Environment (BLADE) in 2018.  
Not only does BricsCAD support both Lisp and DCL in all versions, it can be used across all platforms (Windows, Mac and Linux).  
Recently AutoCAD improved their support for Lisp and DCL to enable use across Windows, Mac and AutoCAD LT.  



### AutoLISP Future

Lisp has outlasted VBA as an API for CAD applications and even without further development of the core language from AutoCAD, the future of Lisp for CAD looks bright, as other players such as BricsCAD take up the slack and continue to promote, develop and push Lisp forward.


## Lisp Basics

Lisp, short for LISt Processing is one of the oldest programming languages.<br>
While it is primarily considered to be a functional language, it has been extended to be whatever is required, including an Object Oriented (OO) language.


### Lisp Functions

To a programmer starting out in Lisp it takes a while to get used to the syntax and naming conventions used within the language. Where:

- `length` - returns the length of a list.
- `strlen` - returns the length of a string.

Part of the problem is that the brevity of function naming is getting in the way of understanding of the functions and their actions.


### Function Renaming

Taking cues from Scheme, a Lisp dialect known for its structured approach to function naming, Lisp can be transformed to the point where code becomes easier to read and understand.

- `length` becomes `list-length`
- `strlen` becomes `string-length`

If applied rigorously, as within **SOZ**, reading Lisp code can become easier to understand and also to program. 

Not only that, it also leads to an understanding that Lisp code can be considered to be Object-Oriented code in disguise as Lisp code can easily be turned into a more readily recognisable format for Object-Oriented method application:

`(SZOB-Apply object method args)`

In SOZ, it doesn't matter which format you use for method invocation, however to remain in the spirit of Lisp many Apply calls have been rewritten to the purely functional format:

`(defun SZOB-length (o) (SZOB-Apply o "length" nil))`

Which then enables the function to be used normally within lisp to do things such as find the sum of all lengths of lines within a list, in just one line of code:

`(apply '+ (mapcar 'SZOB-length line-lst))`


## Types

In **SOZ**, a Type is just another name for a Class.  

There are three main distinctions between types:

- Values - which return a Value as their result
- Objects - which return an **ID** of an object as their result.
- Scripts - which just are run for their internal results.

<br>**SZOBBase** is the base type for all of **SOZ-LIVE**.  

The Base hierarchy of Types for the Project is:

- [SZOBBase](/classes/SZOBBase.html) - Abstract Base class.
  - [Lisp](/classes/Lisp.html) - Abstract Lisp Value Class
  - [SZOBObject](/classes/SZOBObject.html) - Abstract Object Class
  - [SZOBScript](/classes/SZOBScript.html) - Abstract Script Class

The full hierarchy of **SOZ-LIVE** is listed [here](/repos/soz-live.html).

