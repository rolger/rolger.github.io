---
layout: default
parent: Unit Testing
grand_parent: Learning Hours
title: Structuring Unit Tests
nav_order: 1
---

# Structuring your Unit Tests


## Schedule
- 5 min connections: Test Automation Quiz
- 10 min concepts: Testing Theory
- 45 min concrete: Gilded Rose
- 5 min conclusions: Debrief the Gilded Rose

## Connections: Test Automation Quiz 
https://www.menti.com/3ug5i8rx52

## Concepts: Testcase naming strategies
Start with AAA - given / when / then. 
* Given: describes the **initial state** or fixture of the testcase's system under test (= SUT)
* When: the **action** excecuted by the testcase
* Then: the **result** which is expected

Demonstrate different naming strategies. Discuss pros and cons with the participants.

Rules: avoid noise in test names!

## Concrete: 
How should our unit test code reflect AAA?

* one line of code for each
* 1 line of code per A
* multiple lines of code per A

## Concrete Example: Gilded Rose
Select a naming strategy and adapt your code from a previous example. 

Add a **constraint**: The names of the testcases must be at least 30 characters long.

TODO:
Prepare a bad example and let the participants refactor the existing unit tests.

## Conclusions: Unit Testing in the real world
Ask them which strategy are the following? Why did they 
