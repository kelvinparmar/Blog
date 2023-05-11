---
title: "JavaScript variables 101"
datePublished: Wed May 10 2023 06:59:06 GMT+0000 (Coordinated Universal Time)
cuid: clhhco0bq000m09ma05t8cta7
slug: javascript-variables-101
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1683771362717/130eb944-ef8a-4bde-9efa-8555b69d52b9.png
tags: blogging, javascript, wemakedevs, devsintechblogs

---

In this blog, we will go over what variables are, how to declare and initialize them, and how to use them in JavaScript.

# What are Variables?

Variables are containers that hold data values in a program. They are used to store and manipulate data values, which can be of different types, such as numbers, strings, booleans, objects, and more. JavaScript is a loosely typed language, which means that you don't have to specify the type of data you want to store in a variable explicitly.

# Declaring and Initializing Variables

Declaring a variable in JavaScript means defining its name and type. You can do this using the let, const, or var keywords.

The let keyword declares a block-scoped variable. It means that the variable is only accessible within the block of code in which it is defined.

`let age;`

The const keyword also declares a block-scoped variable, but once a value is assigned to it, it cannot be changed.

`const pi = 3.14159;`

The var keyword declares a variable globally, or locally within a function. However, unlike let and const, var is not block-scoped, which means that a variable declared with var is accessible outside the block in which it is defined.

`var name = "John";`

Initializing a variable means assigning a value to it. You can do this when declaring the variable or at any point in the program.

`let age = 25;`

`const pi = 3.14159;`

`var name = "John";`

Using Variables

Once you have declared and initialized a variable, you can use it in your program. To use a variable, you simply call its name.

`let age = 25;`

`console.log(age);` // Output: 25

You can also perform operations on variables. For example, you can add or subtract numbers, concatenate strings, or compare values.

`let age = 25;`

`age = age + 1;`

`console.log(age);` // Output: 26

`let name = "John";`

`let lastName = "Doe";`

`let fullName = name + " " + lastName;`

`console.log(fullName);` // Output: "John Doe"

`let x = 5;`

`let y = 10;`

`console.log(x < y);` // Output: true

# Conclusion

Variables are a crucial concept in programming and JavaScript. They allow you to store and manipulate data values and make your programs dynamic and flexible. As a newbie in tech, understanding how to declare, initialize, and use variables will help you to start building more complex programs.