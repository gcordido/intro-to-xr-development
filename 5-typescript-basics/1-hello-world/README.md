# Hello World

## Objectives

- Download and install the necessary software to start a TypeScript environment.
- Identify the different components of a TypeScript application.
- Create and run a "Hello World" TypeScript application.

## Introduction

TypeScript is a superset of the JavaScript language, which adds additional syntax to support a better integration with editors and code readability by adding types and error catching at compile time, rather than build time. Moreover, as TypeScript code converts to JavaScript after compiling, it is fully compatible with all JavaScript libraries and frameworks, while also running anywhere JavaScript runs. We will be learning TypeScript as our primary programming language to create XR experiences in the web, as it represents a more beginner-friendly approach and can seamlessly implement the (originally created in JavaScript) Babylon.js web rendering engine.

### Understanding Input and Output

Input and Output represent the most basic concepts of programming, as computers receive instructions (**input**) and programs execute them to produce a result (**output**). Though the format in which these instructions are received may vary, the general concept remains the same. In C#, basic output is shown through the **console window**.

```typescript
console.log("Hello World!");
```

What this snippet does is instruct (input) the computer to *print* the message inside the parenthesis as a new line in the console window (output).

There is no need to delve much deeper than that, but it would be useful to keep track of patterns (like the semicolon at the end of the line), as these will come into play later.

### Errors

Errors are bound to happen while writing code, and this is a non-avoidable fact. Thankfully, these are bound to be solvable as well. Early on, the most common errors will have to deal with **syntax** which are the rules, keywords and operators that dictate how the language is written.

```typescript
console.Log("Hello World");
```

This code produces an error (shown by the red, squiggly line underneath *Log*) given that `Log` is not defined as a property of console. The case (lowercase or uppercase) of the letter **L** is different and therefore considers `console.log` and `console.Log` to be different.

Some common errors to avoid early on:

- Mixing lower-case letters instead of capitalizing when needed.
- Writing a comma instead of a period between `console` and `log`
- Adding spaces outside of quotation marks.
- Forgetting double quotation marks (at the beginning and at the end) of a string.
- Forgetting the semi-colon (;) at the end of a command

### Comments

When writing code in TypeScript, any instruction prefaced by `//` or block surrounded by `/* */` is ignored by the computer, does not output in the console window, and is considered a code comment. These come in handy when testing new ways of writing code, as it allows for older pieces of code to remain in our program without needing to delete them.

```TypeScript
// The command below prints the string Hello World.
console.Log("Hello World");
```

Moreover, these are particularly useful to leave notes to ourselves or others who might read our code in the future. Though the syntax might be the same, the way code is written can vary from person to person, so explaining our thought process or what a certain piece of code is doing is always recommended as a good practice.

## Post-Lecture Quiz

## Review and Self Study

We've identified the following resources to provide additional context and learning for the content reviewed in this lesson. We encourage you to review the material below and explore additional related topics.

- [Get Started with TypeScript - Microsoft Learn](https://docs.microsoft.com/en-us/learn/modules/typescript-get-started/);
- [TypeScript: JavaScript with Syntax for Types](https://www.typescriptlang.org/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)