### Day One: What resources / what do I need to learn (Move to a folder)

Time Spent on Day One: XXX

Goals for Day One

- [ ] Figure out the main resources
- [x] Figure out the cirriculum
- [x] Start understanding the data structures etc.

Completed

- Used ChatGPT to summarise a 1H Youtube Video Course + understand the notes
- Speed 2x watched another YT tutorial

---

### Learnings.

Summarize varibles + other data tyes.

- immutable `variables`.
- integer data types are like Solidity `u64`, `i32` + floating numbers such as `f32`, `f64` -`compound data types`: arrays + tuples.
- `const` are fixed
- standard conditionals: `if`, `else`, and `else if`.
- Loops: `loop`, `while`, and `for`. + `break` and `continue`
- Tuples: ordered collection of fixed-size items. Array + tuples are different.
- `Enums`: type that represents a short value. Similar to Solidity.

Tuples + Array Difference.

- Types: Tuples (T) can have different types but arrays (A) has one type
- Size: T has a fixed size
- Indexing: `tuple[(2)]` vs. `array[2]`
- Mutability: Both M + IM

What is a trait in a Tuple / Array

- Trait: features of types
- `Copy`: Copy directly + no extra allocation of memory
- `Clone`: Copy directly + extra allocation of memory
- `IntoIterator`: Value turns into a iterator which is a type that produces sequence of values one at a time.
- Other traits but the above are the basics.

`IntoIterator` usage

```
let array = [1, 2, 3];

// Convert the array into an iterator
let mut iterator = array.into_iter();

// Use the iterator to access the values in the array
assert_eq!(iterator.next(), Some(1));
assert_eq!(iterator.next(), Some(2));
assert_eq!(iterator.next(), Some(3));
assert_eq!(iterator.next(), None); // The iterator is exhausted
```

Installation

- Easy install on various platforms.
- Similar to `C` with the `rustc main.rs` + `./main` execution command.
- Cool first Rust Program. Also looks the same as per the Rust Docs.

---

### ChatGPT Prompts

### [Rust Language 🦀 Crash Course](https://www.youtube.com/watch?v=nweNM-TQYfs)

1 hour video course.

1. I tried to copy and paste the transcript + askeds summarise this `...text...`. But was getting annoying + too long.

```
In this video, the speaker introduces Rust programming language and provides a tutorial on how to install it. Rust is a compiled programming language that aims to provide high-level simplicity with low-level performance, making it a good choice for systems where performance is critical, such as operating systems or game engines. One of the distinctive features of Rust is its memory management techniques, which use a concept called ownership and borrowing to automatically deallocate memory when a variable goes out of scope. The speaker also mentions Rust's package manager called Cargo, and recommends Visual Studio Code as a code editor for Rust development.

In this video, the speaker provides a tutorial on how to install Visual Studio Code and some recommended extensions for Rust development, such as Rust Analyzer and Rust Extension. They also demonstrate how to create and run a Rust program that prints "Hello, World!" by using the Rust compiler and an executable file. Finally, the speaker mentions that in a real-world Rust application, it is more common to use the package manager called Cargo to create a project.

In this video, the speaker continues their tutorial on Rust programming by discussing different primitive data types, such as integers and floating point numbers, and how to declare variables in Rust. They also demonstrate how to use the print and println functions to output text to the console and how to use placeholders to print the values of variables. Finally, the speaker introduces the concept of type inference, which is when the Rust compiler can automatically infer the type of a variable based on the value assigned to it.

In this video, the speaker continues their tutorial on Rust programming by discussing how to declare mutable and immutable variables and how to change the value of a mutable variable. They also demonstrate how to print strings, characters, and boolean values, and how to use placeholders to print the values of variables. The speaker introduces several math operators, including basic arithmetic operators and the modulus operator, and provides examples of how to use them. Finally, they demonstrate how to declare and use float data types in Rust.

```

2. So decided to copy + topic in the Youtube Timestamp: Summarize Variables and Data types, Constants, Conditionals , Loops / Break and Continue, For Loop , while Loop , tuples and Enums in Rust programming language for a mid level developer

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

What is the difference between a tuple + array in Rust programming language?

```
In Rust, a tuple is a fixed-size collection of values with different types. Tuples are often used to store related pieces of data, such as a person's name and age. An array, on the other hand, is a collection of values with the same type, stored in contiguous memory.

Here are some key differences between tuples and arrays in Rust:

Size: A tuple has a fixed size, determined by the number of elements it contains. An array has a fixed size as well, but it is specified using a type parameter (e.g., [i32; 5] is an array of 5 i32s).

Types: The elements of a tuple can have different types, while the elements of an array must all have the same type.

Indexing: Both tuples and arrays can be indexed to access their elements. However, tuples use parentheses to enclose their indices (e.g., tuple[(2)]) while arrays use square brackets (e.g., array[2]).

Mutability: Both tuples and arrays can be either mutable or immutable. However, the elements of a tuple are always mutable or immutable as a whole, while the elements of an array can be individually mutable or immutable.

Ownership: Tuples and arrays can both have ownership of the values they contain. However, tuples are typically used when the values have different types and are not intended to be modified, while arrays are used when the values have the same type and may be modified.

Traits: Tuples and arrays have different sets of implemented traits. For example, tuples implement the Copy and Clone traits, while arrays do not. On the other hand, arrays implement the IntoIterator trait, while tuples do not.
```

3. Expand on this please `Traits: Tuples and arrays have different sets of implemented traits. For example, tuples implement the Copy and Clone traits, while arrays do not. On the other hand, arrays implement the IntoIterator trait, while tuples do not.`

```
In Rust, a trait is a feature that a type can have. It defines a set of methods that a type can implement. Different types can implement the same trait in different ways, depending on their specific behavior.

Here is a more detailed explanation of the differences in trait implementation between tuples and arrays:

Copy and Clone: These traits allow a value to be copied or cloned. The Copy trait allows a value to be copied directly, without allocating any additional memory. The Clone trait allows a value to be cloned by allocating new memory and copying the value into it. Tuples implement the Copy and Clone traits because they are fixed-size collections of values that do not have any additional overhead. Arrays do not implement these traits because they are not always fixed size and may require additional memory allocation when they are copied or cloned.

IntoIterator: This trait allows a value to be converted into an iterator. An iterator is a type that produces a sequence of values one at a time, as needed. Arrays implement the IntoIterator trait because they are collections of values that can be iterated over. Tuples do not implement this trait because they do not have a fixed order for their elements and are not intended to be iterated over.

There are many other traits in Rust, and different types implement different sets of traits depending on their behavior. You can learn more about Rust traits in the official documentation: https://doc.rust-lang.org/stable/book/ch10-02-traits.html

```

4. Give an example of `IntoIterator` conversion in Rust

```
Here is an example of using the IntoIterator trait to convert an array into an iterator in Rust:

let array = [1, 2, 3];

// Convert the array into an iterator
let mut iterator = array.into_iter();

// Use the iterator to access the values in the array
assert_eq!(iterator.next(), Some(1));
assert_eq!(iterator.next(), Some(2));
assert_eq!(iterator.next(), Some(3));
assert_eq!(iterator.next(), None); // The iterator is exhausted
```

---

### [Rust Tutorial #1 - Introduction To Rust Programming](https://www.youtube.com/watch?v=T_KrYLW4jw8)

- 2x speed
- Pretty simple: Installation + how to compile a simple rust program
- Similar to C with the `rustc main.rs` + `./main` execution command.
- Cool first Rust Program. Also looks the same as per the Rust Docs.

---
