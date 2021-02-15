---
layout: default
title: Configuration
nav_order: 2
---

# Configuration

## Connections

1. Read the terms on the board (cards) and arrange them into three categories. 
2. Describe the purpose of the categories in a sentence


* Noise
  * Layouting 
    * Use Braces
    * Group with newline
    * Code Symmetry
    * Group Parameter Validation by Order
    * Favor String.format() over operator '+'
    * Use Guard clauses to fail fast
    * Follow Java naming conventions
    * Follow setter/getter naming conventions
  * Avoid unneccessary code
    * Use Java API instead of do-it-yourself
    * Favor for-each loops
    * Remove unneccessary comparisions
    * Avoid temporary variables instead return a boolean directly
  * Remove dead code
  * Avoid deep nesting levels
  * Remove obvious comments
  
* Principle of least suprise (= POLS)
  * Misleading names
  * Remove wrong comments
  * Avoid mixing sideeffects with business logic

* Complexity
  * Don't implement clever code
  * Split long methods
  * Names should describe the context
  * Avoid deep nesting levels
  * Replace magic numbers with constants and enums
  * Avoid nagations in conditional expressions
  * Avoid conditional complexity
  
