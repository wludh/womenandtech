# Coding 101

## What is coding?

(This [introduction to coding](https://gitpitch.com/ZoeLeBlanc/Coding_101) is adapted from a presentation by Zoe LeBlanc and the UVa Scholars' Lab)

A little less this...

![gif of a dude in a trench coat running around a Best Buy typing on all the computers](https://media.giphy.com/media/eCqFYAVjjDksg/giphy.gif)

... and a little more this...

![gif of Sabrina zapping the radio to life](https://media.giphy.com/media/8caruE0ll6LPPQpF7e/200w_d.gif)
![gif of Sabrina zapping the radio to life](gifs/sabrina.gif)

### What is a computer even?

[Paul Ford **What is Code?**](https://www.bloomberg.com/graphics/2015-paul-ford-what-is-code/#lets-begin)

### Binary/0 & 1

- Way of counting, just like our way of counting that uses the digits 0-9
- Turns our commands into machine readable language
- ["Bits, Bytes, Building With Binary" by Vaidehi Joshi, BaseCS Blog](https://medium.com/basecs/bits-bytes-building-with-binary-13cb4289aafa)

### So, what is code?

- Code tells a computer a set of commands that you want the computer to execute
- Code can be written in many different programming languages
- Code is translated into binary through a compiler or an interpreter and a computer reads the binary

### Women are coders, too

![gif of the girl from Jurassic Park sitting down at a computer](https://media.giphy.com/media/E1Kd3pQwrsMtQbNkt0/giphy.gif)

In fact, the first computer programmer was a woman: Ada Lovelace.

- [Albert Palka, "The Untold History of Women in Software Development"](https://medium.com/codequest/the-untold-history-of-women-in-software-development-299ddc80dd80)
- [Betsy Morais, "Ada Lovelace, teh First Tech Visonary"](https://www.newyorker.com/tech/annals-of-technology/ada-lovelace-the-first-tech-visionary)
- [Laura Sydell, "The Forgotten Female Programmers Who Created Modern Tech"](https://www.npr.org/sections/alltechconsidered/2014/10/06/345799830/the-forgotten-female-programmers-who-created-modern-tech)

![gif of the women from Hidden Figures walking down the hall, with the caption, "Okay ladies, now let's get information"](https://media.giphy.com/media/xThtajIXd9PxmJFxAY/giphy.gif)


## What is Python and how do I use it?

- Python is the programming language we're going to be learning today. It was created in 1991 by Guido van Rossum
- It's named after Monty Python
- It's used for a wide range of programming, from making web apps to data analysis

### Why Python?

"Python is almost always the second best language for any problem"

![gif of Nick Scratch saying, "Conjuration. Demonology. Invocation. Ritual Magic."](https://media.giphy.com/media/1mglCujdwXDvKPqGF3/giphy.gif)

### How do I use Python?

One of the things that's great about Python is that's it's easily readable and understandable for humans. But, as we've discussed, computers don't understand language--they understand `0's` and `1's`. In order to run a program you've written in a high-level language like Python, you need an intermediate program to convert your source code into binary code that the computer can understand. This program is called an *interpreter*.

You can install Python and an interpreter on your own computer (if you're using a Mac, you already have both Python and an interpreter), but there are a number of steps involved. Because we want to get started right away, we'll be using an online interpreter. This allows you to write and run Python code without installing it on your own computer. We'll be using [repl.it](https://repl.it/).

## Let's get started

First, we need to set up our programming environment. Log in to [repl](https://repl.it/) using the username and password you set up earlier. Click on the red plus sign in the lower right hand corner, and then choose "Python" from the list. Give your repl a name ("Coding 101" should work). You're ready to go!

To write a program, you need to give the computer instructions in a format that it understands--in this case, the syntax for Python. Python has built-in functions that you can use to do almost anything you could imagine. But one of the most basic, and important, functions is to print something to the user's display.

`print()`

Whatever you enter between the parentheses is what will be printed for the user (there are some rules, but we'll get to those later). If you want to print words (what we'll call a *string*), then you need to surround those words with quotation marks.

### Try it out

Write your first program by copying the following code into your interpreter and clicking "Run":

`print("Hello, world!")`

Congratulations, you've written your first code!

![gif of Roz and Sabrina high-fiving](https://media.giphy.com/media/1fgKcUz0DYyKZd0YpJ/giphy.gif)

## Variables and data 

Printing is great, but it's only going to get you so far. You're probably going to want to save and manipulate information--names, ages, favorite animals, secrets, weaknesses, and so on. We save information to variables. To create a variable in Python, all you have to do is give it a name and declare its value using an equals sign.

`greeting = "Hello, world!"`

Once you've created a variable, you can use the variable name to access its content.

`print(greeting)`

Notice that we didn't need quotation marks around `greeting`. That's because `greeting` is a variable, and can be called without using quotation marks. In our earlier `print` statement, we were printing a *string*, which requires quotation marks. As we noted earlier, a set of characters other than numbers is called a *string*. Strings need to be surrounded by quotation marks, and can contain any type of character, including letters, numbers, spaces, and special characters.

```
numone = "one"
numtwo = "two"
numthree = "three"

print(numone)
print(numtwo)
print(numthree)
```

Strings aren't the only kind of data type. You can store and manipulate numbers using two data types: *integers* and *floats*. An integer is a whole number, positive or negative, and a float is a number that includes a decimal.

```
numone = 1
numtwo = 2.2

print(numone)
print(numtwo)
print(numthree)
```

What happened to the strings we stored in `numone` and `numtwo`?

![gif of Sabrina looking confused](https://media.giphy.com/media/1SFqe2u1YiSuP8bAD6/giphy.gif)

When we reassigned the variables, we erased the strings that were stored there.

### Joining variables

You can join variables together using the `+` sign. If your variables are integers and/or floats, the `+` operation will add them together:

`print(numone + numtwo)`

But what if one of your variables is a float or an integer and the other is a string? You can't add letters and numbers.

`print(numtwo + numthree)`

You absolutely can't. You can, however, join two floats together. This is called *concatenation*.

```
name = "My name is Sabrina."

print(greeting + name)
```

Why isn't there a space between the two sentences?

Concatenation joins variables exactly as they are. If there isn't a space in the string, then there won't be a space in the concatenated string.

### Try it out

Add a space between "world!" and "My". Then save the concatenated sentences to a new variable called `full_greeting`.

### Naming variables

What happens if you try to use a number for your variable?

`1 = 1`

You'll get a syntax error! That's because Python has rules for how to name variables.

- A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume)
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive (age, Age and AGE are three different variables)

So our previous example could work if we changed the variable name to:

`one_1 = 1`

## Input 

So far, we've assigned values to variables ourselves. But what if we want to let the user input what a variable should be? 

![gif of Prudence crossing her arms and saying, "I'm listening"](https://media.giphy.com/media/ctMRiISeVPUIrJGOnu/giphy.gif)

Python has a built-in function for getting input from the user: `input()`

To use the input function, you'll have to assign the answer the user generates to a variable:

`answer = input()`

You'll also want to print a statement that tells the user what kind of information to input. For instance:

```
print("How much wood could a woodchuck chuck if a woodchuck could chuck wood?")
answer = input()
print("A woodchuck could chuck " + answer + " much wood.")
```

### Try it out

Write a program that asks the user for their name and then greets them using their name.

## Arithmetic

### Try it out

The Spellmans are buying a new TV. The last one was way too small for their enormous, creepy mansion. Write a program that helps people choose the right TV by asking how far the distance between the couch and the TV will be and returns the best screen size.

What you need to know:
- The formula to determine the right size TV is TV = D/2.5, where TV is the ideal screen size and D = distance in inches

![gif of Sabrina and Roz holding hands and acting excited](https://media.giphy.com/media/YUxesd5TB5C809cc7j/giphy.gif)

## String methods

### Try it out

Sabrina is having a sleepover and is preparing some games. Write a mad libs program for the guests to play. Ask the user for at least one verb, one noun, and one adjective, and one curse word, and then use those choices to fill in the blanks in a story that the program prints out. Add some drama to the story by printing the curse word in all caps.

![gif of Aunt Zelda saying, "Praise Satan."](https://media.giphy.com/media/X9GWUOYngS0e4mL43W/giphy.gif)

## Conditionals

### Try it out

Mad libs was a hit, but the guests are getting restless. Write another story, but this time, give the user more control by letting them choose your own adventure. The adventure doesn't *have* to be scary, but that's always an added bonus.

![gif of Ambrose saying, "Spooky."](https://media.giphy.com/media/C9Mi8c9jYXvNvvIE0Q/giphy.gif)

## Loops

### Try it out
Sabrina is casting a spell that requires her to write out the name of a demon over and over and over and over again. Write a program to automate this part of the spell by asking for the demon's name and the number of repetitions required, and then printing the name the requested number of times.

![gif of Sabrina, Nick, and Prudence chanting, "Rise, Rise, Rise"](https://media.giphy.com/media/c7NW30zHO9vt0eKUwJ/giphy.gif)

## Functions

codeacademy order:
- print
- strings and concatenation
- errors
- variables
- arithmetic
- updating variables
- comments
- numbers (integers and floats)
- two types of division/float()
- multi-line strings
- booleans
- valueerror
- strings
- escaping characters
- access by index
- string methods
- lower()
- upper()
- str()
- dot notation
- printing strings
- printing variables
- string concatenation
- explicit string conversion
- string formatting with %

