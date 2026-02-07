---
layout: post
author: Tim_M
---

The **SOZ-LIVE** project contains a large amount of code. But is the size of the project justified? 

Lets first look at the aims and objectives of the project:

## Aims and Objectives

The aims of the project are five-fold:

- to create parametric 3D Solid models and geometry.
- to program using **SOZ** ideas.
- to program in LISP.
- to use a consistent User Interface (UI).
- to create a Node based UI - **LIVE**.


### Parametric 3D.

Currently, the code required for the drafting and modelling of entities and associated parametric objects requires 14000 lines of code (loc).
While being by far the largest portion of the project - this is the main reason why the project exists in the first place.


### SOZ Programming Ideas.

Programming using **SOZ** provides a means to do Object Oriented Programming (OOP) within a Functional Programming (FP) / Scripting Language.
Because of the lack of functionality within the language - all of this has to be coded. The core of **SOZ-LIVE** requires around 3000 loc.  
Together with over 2000 lines of Class and Method Make that enable **SOZ-LIVE** to work, that is a total of around 5000 loc to achieve this aim alone.


### Using LISP.

While the whole project is written in LISP, a portion of it is programming LISP in a **SOZ** format to be used within the project. 
Also included in this are the basic geometric contructs and routines used for types such as Vector, Point, Plane, TMatrix, Line, Curve etc.
This totals around 2000 loc.


### Consistent UI.

Programming the consistent Graphical UI (GUI), while directly supported from **SOZ** programming, still requires significant coding to achieve.
Combined with user selection methods and related routines, this equates to around 3000 loc.


### Node UI - LIVE.

The addition of the Node-based UI - **LIVE** into the project has been achieved using only around 1000 loc.


## Conclusion

Yes, there is a lot of code, but given the functionality and cohesive nature of the project, not only is the size of the project justifiable, but to achieve the Parametric functionality and **LIVE** UI (around 15000 loc), without using **SOZ**, LISP or a consistent UI (a total of around 10000 loc) I believe would take much more coding and effort.
