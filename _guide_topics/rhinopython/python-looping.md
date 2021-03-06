---
title: Python Looping
description: This guide is an overview of looping through Python code.
authors: ['Dale Fugier']
author_contacts: ['dale']
sdk: ['RhinoPython']
languages: ['Python']
platforms: ['Mac', 'Windows']
categories: ['Fundamentals']
origin:
order: 7
keywords: ['script', 'Rhino', 'python']
layout: toc-guide-page
---


## Overview

Looping allows you to run a group of statements repeatedly.  Some loops repeat statements until a condition is *False*; others repeat statements until a condition is *True*.  There are also loops that repeat statements a specific number of times.

The following looping statements are available in Python:

* `for` - Uses a counter to run statements a specified number of times.
* `while` - Loops while a condition is True.
* Nested loops - Repeats a group of statements for each item in a collection or each element of an array.

## For Loop

You can use *for* statements to run a block of statements a specific number of times. For loops, use a counter variable whose value increases or decreases with each repetition of the loop.

The following example causes a procedure to execute 4 times. The *for* statement specifies the counter variable `x` and its start and end values. Python will automatically increments the counter (x) variable by 1 after coming to end of the execution block.

```python
for x in range(0, 3):
    print "We're on loop " + str(x)
```

Python can use any iterable method as a the for loop counter. In the case above we are using `range()`. Other iterable objects can be lists or a string. You can also create you own iterable objects if needed.

Sometimes it is required to increase or decrease the counter variable by the value you specify. In the following example, the counter variable `j` is incremented by 2 each time the loop repeats. When the loop is finished, the total is the sum of 0, 2, 4, 6 and 8.

```python
for j in range(0, 10, 2):
    print "We're on loop " + str(j)
```

To decrease the counter variable, use a negative `range` value. You must specify an end value that is less than the start value. In the following example, the counter variable `j` is decreased by 2 each time the loop repeats. When the loop is finished, total is the sum of 10, 8, 6, 4, and 2.

```python
 for j in range(10, 0, -2):
    print "We're on loop " + str(j)
```

 You can exit any *for* statement before the counter reaches its end value by using the `break` statement. Because you usually want to exit only in certain situations, such as when an error occurs, you could also use the `if` statement in the *True* statement block. If the condition is *False*, the loop runs as usual.

## While Loop

Use the `while` loop to check a condition before each execution of the loop.

```while
var1 = 2
while var1 < 32:
    var1 = var1 * 2
    print var1
print "Exited while loop."
```

*while* loops are not used as much as *for* loops.  But *while* loops are used often in in cases the following way, polling for specific input or a loop that will execute forever until a condition is met:

```python
while True:
    n = raw_input("Please enter 'hello':")
    if n.strip() == 'hello':
        break
```

As you can see, this compacts the whole thing into a piece of code managed entirely by the while loop. Having True as a condition ensures that the code runs until it's broken by n.strip() equaling 'hello'. 

## Nested Loops

Python allows for loops to be nested inside one another.  Any type of loop can be nested within any other type of loop.

```python
for x in range(0, 100):
   if x % 2 == 0:
      print str(x) + " is an even number."
```

---

## Related Topics

- [What are VBScript and RhinoScript?]({{ site.baseurl }}/guides/rhinoscript/what-are-vbscript-rhinoscript)
