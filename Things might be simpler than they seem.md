# Things might be simpler than they seem

| Length | Audience             | YouTube | Held at |
| ------ | -------------------- | ------- | ------- |
| 30 min | Junior - Experienced |         |         |

## Abstract

When you're new to development existing frameworks can seem magical and you sometimes have the feeling that you'll never be able to build something like this on your own.
This talk will take the magic out of a prominent library.
We will look at the basic principles that are used so that you can understand what happens behind the scenes.
With this you will be able to implement it yourself afterwards and maybe even tweak it a bit more.
You are now a library developer!

## Description

In this talk I will implement a very basic version of Redux with the tools that React offers today.
The essence of Redux can be achieved with just a few lines of `useContext` and `useReducer`.
If we sprinkle some types in there as well you get an even better development experience.
With all that in place we can have a look at how we can compose the core building blocks into accessible APIs.

As a tech lead at [Signavio](https://www.signavio.com) I've done this to demystify Redux for junior developers.
We do this in mob-programming sessions where I often as a lot of questions and guide junior developers towards the solution.
This shows them that even very popular libraries can be built using rather simple methods.
I do this to make building new things more accessible.
By regularly showing our junior developers that cool stuff doesn't have to be complicated I encourage them to build new things on their own.

## Outline

### 1. Redux and why it seems so complicated

We shortly explore the redux eco-system.
When people think redux they often immediately also think about libraries such as `redux-thunk` or `redux-saga`.
I want to challenge people to not always start with everything possible but re-evaluate whether they need something or not.
This requires an understanding of what all these extra plugins do.
However, if you're required to understand everything before you start that is a hen and egg problem.
Junior developers sometimes do not fully understand all plugins and therefore it becomes very hard to understand the core.

### 2. Exploring the essence

In this section I will try to peel away the plugins.
I'll do this by providing a short example of what people use a plugin for and why this isn't always necessary.
This should already help the audience better understand the motivation for the talk.

### 3. Redux and React

After we have unraveled everything it is now time to look at the building blocks.
For `redux` I think these are the concept of a `store`, the `connect` method and dispatching actions.
I will highlight how a `store` is also just `state` with some methods on top that you might never need in your application.
We will go on by introducing the `useReducer` hook that will be used for the core.
This hook already gives us most of what we need; a `state` and a `dispatch` method.
Now we only need to make these parts accessible in our application.
For that we can `useContext`.
We're essentially done but I will also show how a `connect` higher-order component, and `reduceReducers` method can be built in just a couple of lines of code.

### 4. Taking this even further

Since we now understand the core of our implementation and have based it purely on standard React functionality we can built even nicer things on top.
I'll show how we can use composition to build some custom hooks for our state.
Given that a TODO app is the standard demo application I will build a `useTodos` hook that features `todos` (the state) and `addTodo` and `removeTodo` handlers that internally connect to the state.
This is an example how knowledge of the core can be used for information hiding.
As the last food for thought I will challenge the idea that an application should only have **one** store.
With our approach we can encapsulate data from each other and only use certain stores when they are really needed.
