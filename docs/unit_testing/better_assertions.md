---
layout: default
parent: Unit Testing
grand_parent: Learning Hours
title: Better Assertions
nav_order: 1
---

# Writing Better Test Assertions
Implement assertions in a none "hard-to-maintain" style.

Thanks to webpapaya: https://dev.to/webpapaya/writing-better-test-assertions-lml

## Schedule
- 5 min connections: Explain the term AAA
- 10 min concepts: Introduce a assertion library like FluentAssertion or AssertJ
- 40 min concrete: example
- 5 min conclusions: What should we take care about in assertions? 

## Connections

Explain the term AAA. What is the purpose of the different phases?


## Concepts

Introduce a assertion library like FluentAssertion or AssertJ.


## Concrete Example

Look at https://github.com/Nagarro-ICAgile-Programming/01-Unit-Test-Assertions.

* Story 1: As shop owner I want to view a list of all employees, which are older than 18 years, so that I know who is allowed to work on Sundays.
* Story 2: As shop owner I want the list of employees to be sorted by their name, so I can find employees easier.
* Story 3: As shop owner I want the list of employees to be capitalized, so I can read it better.
* Story 4: As shop owner I want the employees to be sorted by their names descending instead of ascending.

## Conclusions

What should we take care about in assertions? Note down in your own words what you learnt about a assertions.


```
using System.Collections.Generic;
using System.Linq;
using FluentAssertions;
using NUnit.Framework;

namespace CSharpCore.Test
{
    public class EmployeeReportingTest
    {
        private static List<Employee> BuildEmployees()
        {
            return new List<Employee>
            {
                new Employee("Karl", 54),
                new Employee("Maria", 17),
                new Employee("Anna", 18),
                new Employee("Anton", 16)
            };
        }

        [Test]
        public void older_than_18()
        {
            var employess = FindEmployess(BuildEmployees());
            employess.Should()
                .HaveCount(2)
                .And.OnlyContain(e => e.Age >= 18);
        }

        [Test]
        public void employees_sorted_by_name()
        {
            var employess = FindEmployess(BuildEmployees());
            employess.Select(e => e.Name).Should().BeInDescendingOrder();
        }


        [Test]
        public void employees_name_becomes_uppercase()
        {
            var employess = FindEmployess(BuildEmployees());
            employess.Should()
                .OnlyContain(e => e.Name.All(char.IsUpper));
        }

        private List<Employee> FindEmployess(List<Employee> employees)
        {
            return new List<Employee>(employees
                .FindAll(e => e.Age >= 18)
                .OrderByDescending(e => e.Name)
                .Select(e => new Employee(e.Name.ToUpper(), e.Age)));
        }
    }
}
```