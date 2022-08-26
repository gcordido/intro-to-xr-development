# Variables and Types

## Objectives

- Declare a variable.
- Select the appropriate data type for a variable.
- Recognize the function of the assignment operator.

## Introduction

Programming languages make use of the computer's memory to 'remember' previous information to be used throughout a program's execution, such as specific values, names and inputs. These are stored in allocations of the computer's memory called **variables**.

![Three buckets of different sizes, with the words integer, string and double printed on them.](../../images/variable-buckets.png)

Variables work like a bucket, where once it has been declared (created in programming terms) we can put, retrieve or modify the things in it. However as with a real bucket, its size is important depending on the contents we intend to put in, so variables come in different sizes depending on the type of data we want to store. These  types have their own label and help us declare the appropriate size variable for our uses.

### Declaring a variable

**Declaring** a variable means telling the computer to allocate space in its memory large enough to hold the specific type of data by the label. In TypeScript, variables can be initialized through the `var` and `let` keywords. Though there are specific cases for each, we will focus on using `let`.

Here we declare two variables to store numbers:

```typescript
let x: number;
let y: number;
```

At this time, these variables are just two empty spaces. We can assign (store) values to this allocated space in memory using the `=` sign. In most programming languages, the equal sign is known as the assignment operator. This means it does not work the same way it works in regular math, and what it does is store a value inside a variable.

```typescript
//Storing the number 4 in variable x
let x: number = 4;

//We can also store a value resulting from a mathematical operation, let's try storing the value of x + 2 in y
let y: number = x + 2;

console.log(y);
```

What our program is doing here is storing the number 4 in our variable `x`, and storing the value of `x + 2` *(4+2)* in our variable `y`.

Once the variables have been declared, the type label is no longer necessary.

### Constants

A constant is a variable whose value cannot be modified. These are declared using the keyword `const` and must always be declared with an initial value (i.e. it cannot be empty).

```typescript
const c: number = 10;

//If we tried to reassign the value of "c" it would return an error
c = 12;
ERROR Cannot assign 'c' because it is a constant.
```

### Simple Types

However, we may not always want to deal with numbers. TypeScript offers various different types that we can use, depending on what we need our program to do.

The following list covers the simple types, that is, the most primitive types that TypeScript offers:

```typescript
let variable1: number = 10;
let variable2: boolean = true;
let variable3: string = "Hello World";
```

- The first variable is the type we declared previously, **number**. This data type is used when working with whole numbers or floating points (decimals).
- The second variable is called a **boolean** variable. It holds one of two possible values: *True* or *False*, and it's used as a condition marker.
- The last variable is called **string**. This type is used to store text values, which are always enclosed in quotation marks.

### Special Types

TypeScript features some types that can be used when we may not need to refer to a specific kind of data.

```typescript
let variable4: any;
let variable5: unknown;
```

- The first variable in this case is of type `any`. **Any** is a type that disables type checking and allows all types to be used. This means you can technically change the contents of the variable from one data type to a different one without running into an error.
- The second variable is a safer alternative to `any`, called `unknown`. **Unknown** is best used when we do not know the type of the data being assigned.

The key difference between `any` and `unknown` is that after the variables have been assigned a specific value, the `any` type can be assigned to anything and may call methods or constructors (seen later) at the expense of running into errors that could technically be prevented. While `unknown` cannot be assigned to anything unless its type is changed before, which allows to remove unexpected errors in advance.

## Post Lecture Quiz

## Review and Self Study
