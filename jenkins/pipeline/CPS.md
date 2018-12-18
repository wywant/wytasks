
# Continuation
In wikipedia, [continuation](https://en.wikipedia.org/wiki/Continuation). 
```
 a continuation is an abstract representation of the control state of a computer program.
```
```
Continuations are useful for encoding other control mechanisms in programming languages
such as exceptions, generators, coroutines, and so on.
```
In [The Javaflow Component](http://commons.apache.org/sandbox/commons-javaflow/)
```
Think of a continuation as an object that, for a given point in your program, 
contains a snapshot of the stack trace, including all the local variables, and the program counter. 
You can not only store these things in the continuation object, 
but also restore the execution of the program from a continuation object.
```
