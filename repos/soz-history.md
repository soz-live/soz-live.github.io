---
layout: default
description: Sub Repo, with History functionality included.
type: Private
status: Beta
---

# soz-history

## Introduction

The **soz-history** repo adds history functionality to **SOZ**.

With this repo it is possible to record a state of drafting / design, at a specific TimeStamp, that enables the user to return to that state and can be recalled later for whatever reason.  
<br>
To record a state, use the H-Record command.  
To recall the first state, use the H-First command.  
To recall the last state, use the H-Last command.  
To recall a state, use the H-Select command.  

## Class Hierarchy

- [SZOBBase](/classes/SZOBBase.html)
  - [SZOBObject](/classes/SZOBObject.html)
    - [SZOBHistory](/classes/SZOBHistory.html)
      - [SZOBHistory-Record](/classes/SZOBHistory-Record.html)
        - [SZOBHistory-RecordObject](/classes/SZOBHistory-RecordObject.html)
          - [SZOBHistory-RecordObject-Now](/classes/SZOBHistory-RecordObject-Now.html)
      - [SZOBHistory-RecordObjects](/classes/SZOBHistory-RecordObjects.html)
      - [SZOBHistory-TimeStamp](/classes/SZOBHistory-TimeStamp.html)
        - [SZOBHistory-TimeStamp-Now](/classes/SZOBHistory-TimeStamp-Now.html)

Version:  1.27.0
<br>
Date: 20251204.2009
