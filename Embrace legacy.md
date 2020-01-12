# Embrace legacy

| Length | Audience               | YouTube                                             | Held at                                                                                                                                                              |
| ------ | ---------------------- | --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 30 min | Beginner - Experienced | [Link](https://www.youtube.com/watch?v=tFHJD1ciB7M) | [Signavio](https://www.signavio.com) Tech Talk, [HPI](https://hpi.de/plattner/teaching/archive/winter-term-201718/softwaretechnik-ii.html) Softwaretechnik II course |

## Abstract

The moment you write a line of code you are putting an expiry date on it.
There is only one way of pushing this expiry date further into the future: refactoring.
While some changes are small others require to completely change the tech stack.
But how can you make these changes without putting development on halt?
This talk will show you how to continuously improve a code base without making everyone hate you.

## Description

In this talk we will be looking at the structure of applications and the different kinds of changes can make to it.
We will explore how you need to understand the structure of the application in order to make changes to it in a reasonable way.
First we play through a change that seems small at first but keeps on growing until half the application is changed and merge conflicts becomes your daily business
After that we look at what went wrong and how we could improve our strategy.
This is supposed to show the audience that every large problem can usually be split into a set of very small problems.
By doing this we can make the hard become easy.
I'll also show how this approach helps you to embrace changes instead of fearing them.

## Outline

### 1. What is legacy

I will use this section to create a shared understanding of legacy code.
What is surprising to many people that legacy code does not have to be bad code.
Even code written with the best of intentions becomes outdated and hard to maintain over time.

### 2. Introduction of the "straight forward" method

I will show how a change might be implemented when the developer does not think about the underlying system.
This will be highlighted by playing through "bug reports" while the system is being changed.
I will show how long lasting big changes lead to more problems than they solve.

### 3. Tackling changes bottom-up

We will then look at a different approach which takes the problem apart.
By tackling changes one at a time I will highlight how we keep everything operational while still being able to quickly respond to problems.
This should also highlight how everyone can be relaxed at every stage of making the change.

### 4. Recap and wrap-up

I briefly go over the main differences of the two approaches.

## Related material

- [Ryan Florence - Don't Rewrite, React!](https://www.youtube.com/watch?v=BF58ZJ1ZQxY)
- The Mikado Method ([Book](https://mikadomethod.wordpress.com/), https://pragprog.com/magazines/2010-06/the-mikado-method)
