---
layout: default
parent: Test Driven Development
grand_parent: Learning Hours
title: Out-Side-In
nav_order: 1
---

# Finding examples for in-side-out TDD
Designing an API of collaborators driven by test 


## Connect
Ask the following question: Which terms came into your mind about TDD?


## Concepts
Explain the different TDD styles


## Concrete
Present the following kata to the paritcipants:

Shipping Cost Service

We are going to test drive a service for calculating the shipping cost of a package or letter.

- If the destination country is in the common market, a flat rate of 5 is calculated
- If the destination country is North America and the delivery type is
  - Express: a flat rate of 50 is calculated
  - Standard: a flat rate of 35 is calculated
- Any other country costs the km multiplied by 9% but a minimum of 15

Design with TDD the interface of another service to calculate the shipping costs. This service will use some REST call to retrieve the required information


Introduce this table to document the examples
Ask the participants to find their examples in pairs (just the IN and OUT column)
Ask the participants to design an interface for the geo requests
Implement tests and code

## Conclusions


