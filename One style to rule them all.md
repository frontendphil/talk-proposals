# One style to rule them all

| Length | Audience                   | YouTube                                     | Held at                                                                  |
| ------ | -------------------------- | ------------------------------------------- | ------------------------------------------------------------------------ |
| 30 min | Intermediate - Experienced | https://www.youtube.com/watch?v=Oo_S1MZFEEQ | [React Berlin](https://www.meetup.com/de-DE/React-Berlin-Meetup/) Meetup |

## Abstract

When you're developing a JavaScript library you can declare all you projects' dependencies through your `package.json`.
That is, of course, all except the styles.
Some libraries ship CSS files, some use a CSS-in-JS approach.
However, regardless of the method you need to force the people that use your library to adapt to the decisions you have made.
This talk proposes a new way that lets the people who use your library use their existing styling approach.
All without you knowing what they will opt for in the end.

## Description

In this talk I will explore the underlying principles of style.
I will introduce the different approaches used by different frameworks.
Then I'll create an abstraction that manages to takes advantage of the rules we've learned before.
This means that applying styles can be turned into a concern for the application and not the individual component.
If we handle styles with this approach we do not need to treat them as a special dependency to our projects anymore.

## Outline

### 1. Why is style a dependency?

I will give some examples of how styles are shipped today.
This will be used to show how small decisions by library authors can turn into big burdens of application developers.
I will then look at what the approaches have in common, where they differ, and how we can use that to our advantage.

### 2. How can we turn that around?

Given what we've learned in the beginning I'm going to sketch an API that can be used by components.
We'll learn about some quirks and what we need to do in order to build a declarative API that matches the React paradigms.

### 3. Real world example through `substyle`

In the last part we're going to look at a real world implementation - [`substyle`](https://github.com/jfschwarz/substyle).
Based on an example application I'm going to change the styling approach for the page profoundly while maintaining a consistent look and feel.
This is intended to proof that the method can work and should encourage people to challenge how they think about styles after the talk.

## Related talks

- [Jan-Felix Schwarz - How to Support All Styles of Styling](https://www.youtube.com/watch?v=CKPzyeX7nyA)
