---
layout: default
---

# Basics

## Contents

- Basics
  - [Introduction](#introduction)
  - [Strings vs Symbols](#strings-vs-symbols)
  - [The Meta Environment](#the-meta-environment)
 

## Introduction

This page contains basic information for coders working with **SOZ**.  


## Strings vs Symbols

**SOZ** uses Strings, instead of Symbols, within the code for Arguments, Class, Method and Function names and documentation strings, because:

- converting strings to symbols is easy.
- Users have to be able to read the strings.
- It enables automatic documentation of the system.


## The Meta Environment

The **Meta** Environment exists as a single entity in memory at run-time and stores and indexes all relationships between:

- Classes,
- Functions,
- Methods
- Categories
- Settings

The **Meta** information is accessed to determine things such as:

- Superclass and Subclass information
- Function / Method signatures and their required Types / Classes.

