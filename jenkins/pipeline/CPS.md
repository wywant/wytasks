
# CPS
In wikipedia [Continuation-passing style](https://en.wikipedia.org/wiki/Continuation-passing_style)
```
In functional programming, continuation-passing style (CPS) is a style of programming 
in which control is passed explicitly in the form of a continuation. 
This is contrasted with direct style,
```
```
A function written in continuation-passing style takes an extra argument: 
   an explicit "continuation", i.e. a function of one argument.
```

# Continuation
In wikipedia, [continuation](https://en.wikipedia.org/wiki/Continuation). 
```
 a continuation is an abstract representation of the control state of a computer program.
```
```
Continuations are useful for encoding other control mechanisms in programming languages
such as exceptions, generators, coroutines, and so on.
```
```
The term continuations can also be used to refer to first-class continuations,
which are constructs that give a programming language the ability
to save the execution state at any point 
and return to that point at a later point in the program, possibly multiple times.
```
In [The Javaflow Component](http://commons.apache.org/sandbox/commons-javaflow/)
```
Think of a continuation as an object that, for a given point in your program, 
contains a snapshot of the stack trace, including all the local variables, and the program counter. 
You can not only store these things in the continuation object, 
but also restore the execution of the program from a continuation object.
```
