# Classes and Functions

## Objectives

- Understand what is a function and how to define one.
- Differentiate between existing return types.
- Familiarize with the use of parameters.
- Understand the uses of arrow and asynchronous functions.

## Introduction

There will be situations where we will be required to address different problems separately, with the intent of simplifying our code and enhancing performance. There will also be situations where we may need to re-use a previously developed solution. For both of these cases, TypeScript provides a solution in the form of classes and functions. 

A **class** is a template or blueprint for an object, which in itself encompasses variables, functions and other properties.

A **function** is a block of code that combines different elements (such as variables) to produce a specific result or carry out a specific procedure. These are declared inside of a class, and as such are dependent on it to be re-used.

### Creating Classes and Constructing Objects in TypeScript

To create a class, we use the `class` keyword, followed the class' name and a constructor function, which dictates the default components of the class. We will dive into functions in more detail next. For now, this is the general syntax to create a class:

```typescript
class Dog {
    constructor() {
        //Default components
        this.name: string;
        this.breed: string = "Corgi";
    }
}
```

Each instance (or **object**) of the class uses the skeleton or blueprint provided, but is given its own values that identify it as a unique instance. In the `Dog` class above, we've assigned two attributes. The first is a string for the dog's name and the second is a string for the dog's breed. Essentially, each instance of the Dog class will have a different name. However, the breed for each instance will always be a Corgi.

You may notice we used a keyword when defining this attributes: `this`. **this** is a keyword that refers to the owner of a function (in this case the `Dog` class). We use this to ensure that when initializing an object, we are adjusting that *specific object's properties*, rather than any other object we may have created of that class.

Once the class is created, then objects can be initialized following this syntax:

```typescript
const myDog = new Dog();
myDog.name = "Sushi";

console.log(myDog.breed);
console.log(myDog.name);
//OUTPUT: Corgi
//        Sushi
```

In this case, the object `myDog` is initialized, and the name property is assigned the string `"Sushi"`.
**Note:** We can also define a constructor such that certain attributes (like the dog's name) is given at the moment we initialize the object. This is done via *parameters*. 

```typescript
class Dog {
    name: string;

    constructor(name: string) {
        this.breed: string = "Corgi";
        this.name = name;
    }
}
```

A *parameter* is a value that is passed into a function when called. We will cover this in a bit.

### Declaring Functions in TypeScript

Functions are building blocks, which combine code together to simplify coding. Functions are only run when they are called.

The following is the syntax to create a function:

```typescript
function addTwoNumbers(x: number,y: number): number {
    return x + y;
}
```

An access identifier, which determines whether the function can be used by outside code, can be public or private.
The return type, which depends on the desired outcome of our function. We can return a specific value (by return, programming lingo means resulting in a data value). This will be written as one of the data types we have discussed previously, such as int.
The function name which can be anything, but should aim to make sense with what the function does to make it clearer for anyone who reads the code.
The parameters, which are values or variables that are passed into the function for usage.
The following is the syntax to call a function:


If you don't need the function to return anything (ex: a function that just writes to the console) you can use the return type void. This returns nothing and requires no return statement.

#### Arrow Functions

#### Asynchronous Functions