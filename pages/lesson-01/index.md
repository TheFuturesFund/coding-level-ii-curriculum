---
permalink: "/lesson-01"
layout: "default"
---

# Lesson 1 - Review & intro to programming Ruby

This lesson seeks to review basic programming concepts the students learned in Level I.
In addition, this class seeks to relate those concepts to the Ruby programming language.

## Tools

Lets start by reviewing some of the tools that we as developers have available to us.
We will be using these extensively in this class, and you'll get know them more as we go, but in brief, here they are:s

### The terminal

The terminal is a command line interface that allows you to run commands and interact with your computer at a very low level.

The terminal works inside of *directories*, which are the files/folders you have on your computer.
When you first start your terminal, it begins inside you *home directory*.
My home directory is `/home/jonathan`, but yours is almost certainly different.

To see what your home directory is, you can use the `pwd` command which shows you the current directory:

```shell
$ pwd
/home/jonathan
```

Now that we have our bearings, let's use the `ls` command to see what files are in our home directory:

```shell
$ ls
Design  Developer  Downloads  Pictures  Temporary
```

The list of directories inside your home directory may be different than mine.
Let's pick a directory to explore.
I'm going to use `Developer`, but you can pick an of the ones that appear when you type `ls`.

```shell
$ cd Developer
$ pwd
/home/jonathan/Developer
$ ls
AUR  coding-level-ii-curriculum  jmhooper.github.io
```

Now let's make a directory.
This is the sort of thing we'd have to do when starting a new project.
I'm going to make a new directory in my `Developer` directory using the `mkdir` command:

```shell
$ mkdir my-new-project
$ ls
AUR  coding-level-ii-curriculum  jmhooper.github.io  my-new-project
```

There's a whole lot of other commands we'll be covering in this class.
We'll wait until we're ready to use those before we got into more depth.

### The Text Editor

The text editor is used to edit files on your computer.
The most basic text editors are Notepad for windows computers, and TextEdit for Macs.
There are other more advanced text editors available to use for coding, and we'll use on of those for this class.

Some of the most common text editors include:

- [Sublime Text](https://www.sublimetext.com/)
- [Atom](https://atom.io/)
- [Textmate](https://macromates.com/)
- [Vim](http://www.vim.org/) (Advanced)

## What is Ruby?

From [ruby-lang.org](https://www.ruby-lang.org/en/):

> Ruby is a dynamic, open source programming language with a focus on simplicity and productivity. It has an elegant syntax that is natural to read and easy to write.

## Executing Ruby Code

- REPL
- From a file

## Values

### Numbers

### Strings

### Booleans

### Nil

### Collections

#### Arrays

#### Hashes

## Variables

Variables in ruby work much like variables in other common programming languages.
Variables associate a *name* with a *value*.

Setting a variable's value is called `assignment` and is done with a `=`.
For this reason, in Ruby we call the `=` the "assignment operator".

```ruby
a = 5
b = "The Ruby programming language"
c = false
```

Notice that a variable's value can be assigned many different types of values.
In the example above, `a` is a number, `b` is a string, and `c` is a boolean.

After assigning a variable, you can use it's name later in your program to get it's value

```ruby
a = 5
b = 6
a + b
# => 11
```

## Arithmetic

The most basic thing you can do with a Ruby program is arithmetic, or simple math.
We've already seen this in the example above with `a + b`.
Ruby equips you with many other operators.

Here's a few examples:

```ruby
1 + 2 # Addition
5 - 4 # Subtraction
3 * 3 # Multiplication
4 / 2 # Division
```

Arithmetic operators can be combined with variables to build more complex statements:

```ruby
a = 5
b = 10
b / a
# => 2
```

When doing arithmetic, Ruby respects the order of operations (PEMDAS).
In addition, parentheses are respected in the same way they are in typical algebraic expression:

``` ruby
4 + 3 * 5
# => 23

(4 + 3) * 5
# => 35
``` 

## Logic

## Control Flow

Ruby has a number of statements that allow you add logic to your code to control how it runs.
Using statements that alter the way your code runs based on certain conditions is called "Control Flow"

### If Statements

The most basic element of Ruby control flow is the *If Statement*.
An if statement takes a piece a Ruby expression and evaluates it to determine if it is true or false.
In the case of truth, Ruby can be given a piece of code to execute.

```ruby
a = 4
b = 2 + 2
c = 6

if a == b
  c = 7
end
```

`c` is equal to 7 since a and b are equal.

Additionally, an else statement can be provided that describes what the program should do if the expression is false.

```ruby
a = 4
b = 5
c = 6

if a == b
  c = 7
else
  c = 8
end
```

`c` is equal to 8 since 4 does not equal 5.

### Loops

Ruby implements a number of looping constructs.
These work similarly to for loops in other programming languages.

Ruby does not implement a traditional style for loop, opting instead to encourage the programmer to find a more idiomatic looping construct.

#### While / Until

A while loop executes a block of code until a statement is false.

```ruby
a = 0

while a < 4 do
  a = a + 1
end
```

The block above will run 3 times until `a` is equal to 4, at which point it will stop.

An until loop does the opposite, executing a block of code until a statement is true.

```ruby
a = 4

until a == 0 do
  a = a - 1
end
```

The block above will run 4 times until `a` is equal to 0, at which point it will stop.

#### Times

#### Each

## Functions

## Input/Output (IO)

## Portfolios
