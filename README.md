# crab-stuff
Learning Rust / the crab language

Using ChatGPT to guide me to learn Rust in 30 days. 

Suggestions:
- Rust syntax + basic concepts (variables / data types / control structure & functions)
- Exercises + small projects
- Read other code

---
### Day One: What resources / what do I need to learn (Move to a folder)

Summaries via ChatGPT. 
I pasted the transcript + askeds summarise this ```...text...```
### [Rust Language 🦀 Crash Course](https://www.youtube.com/watch?v=nweNM-TQYfs)
1 hour video course. 

In this video, the speaker introduces Rust programming language and provides a tutorial on how to install it. Rust is a compiled programming language that aims to provide high-level simplicity with low-level performance, making it a good choice for systems where performance is critical, such as operating systems or game engines. One of the distinctive features of Rust is its memory management techniques, which use a concept called ownership and borrowing to automatically deallocate memory when a variable goes out of scope. The speaker also mentions Rust's package manager called Cargo, and recommends Visual Studio Code as a code editor for Rust development.

In this video, the speaker provides a tutorial on how to install Visual Studio Code and some recommended extensions for Rust development, such as Rust Analyzer and Rust Extension. They also demonstrate how to create and run a Rust program that prints "Hello, World!" by using the Rust compiler and an executable file. Finally, the speaker mentions that in a real-world Rust application, it is more common to use the package manager called Cargo to create a project.

In this video, the speaker continues their tutorial on Rust programming by discussing different primitive data types, such as integers and floating point numbers, and how to declare variables in Rust. They also demonstrate how to use the print and println functions to output text to the console and how to use placeholders to print the values of variables. Finally, the speaker introduces the concept of type inference, which is when the Rust compiler can automatically infer the type of a variable based on the value assigned to it.

In this video, the speaker continues their tutorial on Rust programming by discussing how to declare mutable and immutable variables and how to change the value of a mutable variable. They also demonstrate how to print strings, characters, and boolean values, and how to use placeholders to print the values of variables. The speaker introduces several math operators, including basic arithmetic operators and the modulus operator, and provides examples of how to use them. Finally, they demonstrate how to declare and use float data types in Rust.

I couldn't be bothered to copy and paste the rest of the video so looked at the timeline stamping of the YT video + asked for summarises.
``` 
Summarize Variables and Data types, Constants,  Conditionals , Loops / Break and Continue, For Loop , while Loop , tuples and Enums in Rust programming language for a mid level developer
```

```
Sure! Here is a summary of some basic concepts in the Rust programming language:

Variables and data types:

In Rust, variables are immutable by default. To make a variable mutable, you must use the mut keyword.
Rust has a number of built-in data types, including integers (e.g. i32, u64), floating-point numbers (e.g. f32, f64), booleans (bool), and characters (char).
Rust also has compound data types, including arrays ([T; N]) and tuples ((T1, T2, ...)).
Constants:

Constants in Rust are values that are fixed at compile-time and cannot be changed at runtime.
Constants can be declared using the const keyword and must be annotated with their type.
Constants can be declared in any scope, including global and local.
Conditionals:

Rust has the usual conditional statements, such as if, else, and else if.
The condition in an if statement must evaluate to a boolean value.
Loops:

Rust has several looping constructs, including loop, while, and for.
The break and continue keywords can be used to control the flow of a loop.
For loop:

The for loop allows you to iterate over a collection of items.
The syntax is for item in collection, where item is a variable that takes on the value of each element in the collection on each iteration.
While loop:

The while loop repeatedly executes a block of code as long as a condition is true.
The syntax is while condition { ... }.
Tuples:

A tuple is an ordered collection of fixed-size items.
Tuples can contain items of different types.
The items in a tuple can be accessed using indexing.
Enums:

An enum (short for enumeration) is a type that represents a fixed set of values.
Enums can be used to define a type with a small number of possible values.
Each value in an enum is called a variant.
```


---

### Resources

Mandatory
- The Crab Book
- Docs. 

Small exercises
- Rustling
- Rust by Example
