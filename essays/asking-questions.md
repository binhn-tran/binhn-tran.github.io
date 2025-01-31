---
layout: essay
type: essay
title: ""
date: 2025-01-30
published: true
labels:
  - Not so much smart questions
  - Smart questions
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/question.jpg">

## The Importance of Asking Smart Questions in Computer Science

I believe that asking smart questions is important in the field of computer science because it helps you better understand how to assist another programmer in debugging and improving their code. However, asking questions without providing sufficient background information about the issue you're facing is not the best approach.

## Asking the right questions

```
let mode:number = 2;
let level:string = 'pro';

```

[When defining a property in TypeScript using let or otherwise, what is the best practice or rule on defining its type?](https://stackoverflow.com/questions/51930131/when-defining-a-property-in-typescript-using-let-or-otherwise-what-is-the-best)
The user says that they're new to Typescript and asks "What are the rules or best practices for defining a type when declaring a property using let?" They look like they know how to define a type when declaring a property using a let, but are unsure of the rules about it. 

## Why is it a smart question?

This is a good question because it addresses a concern in TypeScript regarding the best practices for defining property types. The user also demonstrates what they have attempted so far and mentions that they are relatively new to TypeScript and is unsure about the rules for defining types. By asking about the best practices for defining property types, the user is highlighting an important aspect of code organization. Being organized is crucial, especially when working on larger projects. When defining a property in TypeScript, it is best to use let, const, or var to declare the type.

## Asking the wrong questions

```
MainCtrl.prototype.addTodo = function () {
    var newTodo = this.$scope.newTodo.trim();
    if (newTodo.length < 10) {
        alert("The input must be longer then 10 signs!");
    }
    this.todos.push(new TodoItem(newTodo, false));
    this.$scope.newTodo = "";
    console.log(todos.length);
};

```

[ReferenceError: todos is not defined Javascript and Typescript](https://stackoverflow.com/questions/47491173/referenceerror-todos-is-not-defined-javascript-and-typescript)
There are several reasons why this is not a smart question. The user wrote code in TypeScript, then compiled it into a .js file and reported an error in the console stating that todos isn't defined. This approach essentially throws code at someone and asks them to figure out the problem without providing enough context or insight into the issue. The question lacks the necessary background information, such as details on how the todos variable is declared or any supporting context on how the code is structured. To improve this, the user should provide more specific information about their issue, such as including the relevant parts of the TypeScript file, what errors they’ve already tried to resolve, and any debugging steps they've taken.

## Why it's a not so smart question

The question presents the code and the error message, but it lacks context that could help others identify the issue. The user doesn’t explain what troubleshooting steps they’ve already taken, or what they’ve tried to resolve the problem. While the user provides links to JSFiddle, they don’t mention whether they’ve tried basic debugging methods, such as checking the console logs or verifying if the variable todos is properly initialized. Without this kind of context, it's unclear if the user has attempted to find a solution on their own or if they’re simply relying on others to do the work. To make the question more effective, the user should clarify how todos is defined, what they've tried so far, or if they’ve consulted documentation or searched for the error elsewhere. Providing this background would demonstrate that they are actively working toward a solution and would make it easier for others to assist them.


## Final comments

To conclude, asking smart questions is an important skill to develop as a software engineer. By asking the right questions, more people in the community are willing to help you, as it shows you're willing to put in the time and effort to learn. However, when you ask the wrong questions, others might think you're expecting them to do the work for you. Additionally, you won't become a better programmer if you don't attempt to solve the issues on your own first.

## AI Use

I used AI to search for a not so smart question, the titles, as well as for grammar checking.
