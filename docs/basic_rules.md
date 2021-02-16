---
layout: default
parent: Clean Code
grand_parent: Learning Hours
title: Basic Rules
nav_order: 1
---


## Schedule
- 10 min
- 5 min
- 40 min
- 5 min

## Connections

Prepare either cards or a Miro board.

Instructions:

1. Read the terms on the board (cards) and arrange them into three categories. 
2. Describe the categories in a sentence

List of statements

| Category        | Statements                 | 
|:----------------|:---------------------------|
| Noise           | Layout and conventions     |
|                 | Avoid unnecessary code     |
|                 | Remove dead code           |
|                 | Remove obvious comments    |
| Principle of least surprise (= POLS) | good and plenty   |
| Complexity      | Dont implement clever code |

* Noise
  * Layout and conventions
    * Use braces
    * Group with newline
    * Lookout for code symmetry
    * Group parameter validation by order
    * Favor String.format() over operator `+`
    * Use guard clauses to fail fast
    * Follow Java naming conventions
    * Follow setter/getter naming conventions
    * Same code formatting rules
  * Avoid unnecessary code
    * Use Java API instead of do-it-yourself
    * Favor for-each loops
    * Remove unnecessary comparisons
    * Avoid temporary variables instead return a boolean directly
  * Remove dead code
  * Remove obvious comments

* Principle of least surprise (= POLS)
  * Name are not misleading
  * Remove wrong comments
  * Avoid mixing side-effects with business logic

* Complexity
  * Dont implement clever code
  * Split long methods
  * Names should describe the context and not the implementation
    * Avoid abbreviations
  * Avoid deep nesting levels
  * Replace magic numbers with constants and enumerations
  * Handle conditional complexity
    * Avoid negations in conditional expressions
  * Avoid deep nesting levels


## Concepts

Present Slides: XP - Rules of Simple Design

Simplicity:  
	- Noise / POLS / Complexity


## Concrete Example

* Clean Code Repo Roland/Martin
    * Stage 5: Layout, Long method, Conditions, Duplication


## Conclusions

Note the rules you applied in this session and which you will apply in future.
