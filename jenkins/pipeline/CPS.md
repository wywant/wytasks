
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
```
When the CPS function has computed its result value, 
it "returns" it by calling the continuation function with this value as the argument. 
That means that when invoking a CPS function, 
the calling function is required to supply a procedure to be invoked with the subroutine's "return" value. 
```

In wikipedia [Direct style](https://en.wikipedia.org/wiki/Direct_style)  
```
In computer programming, direct style is the usual style of sequential programming, 
in which control is passed implicitly by simply going to the next line, 
by subroutine calls, or by constructs such as return, yield, or await. 
It is contrasted with continuation-passing style, 
in which control is passed explicitly in the form of a continuation.
```
```
Every call in CPS is a tail call, and the continuation is explicitly passed. 
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
