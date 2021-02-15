---
layout: default
parent: Clean Code
title: Conditional Complexity
nav_order: 4
---

## Schedule
- 10'
- 20'
- 40'
- 5'

## Connections: Well-known refactoring in my IDE

* Create a list of your most well-known refactorings
* Assign the key binding in your IDE

## Concepts: refactoring conditionals 

### Explain the transformations
Basic idea is that there are different possibilities to transform conditional expressions

* Invert condition with De Morgan�s law
* Invert condition to exchange if and else statements
* Join nested if statements with operator '&&'
* Split long operator '&&' conditions into nested if statements
* Remove unnecessary 'else' statement and use early return statements in 'if' instead
* Multiple 'if' statements with same condition: join code into one block (and reverse - some kind of split phase)
* If there is a duplication inside the if block:
  * Join sequential 'if' statements with with operator '||'
  * Split long operator '||' conditions into sequential 'if' statements with the same block
* Group and order multiple conditions by variable usage
* Replace 'if' with 'switch' and vice versa

### examples of conditional transformations
Mob Programming: examples of conditional transformations

## Concrete Example 

Your task is to refactor the code in the TennisGame2 Kata.

Use the keys for the following refactorings:
- rename variable
- extract method
- extract local variable/field
- inline method/variable
- change signature
    
## Conclusions

What changed ???


Emily Bache: https://github.com/emilybache/Refactor-Conditionals
