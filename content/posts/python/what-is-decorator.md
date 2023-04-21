---
title: "What Is Decorator"
date: 2023-04-20T19:57:26+01:00
draft: true
---
In Python, a decorator is a function or a class that is used to modify the behavior of another function or class without changing its source code. A decorator takes a function or a class as input and returns a new function or class that adds some extra functionality to the original function or class.

Decorators are typically used to implement cross-cutting concerns such as logging, caching, authentication, or performance monitoring, without having to modify the code of the original function or class.

In Python, a decorator is denoted by the "@" symbol, followed by the name of the decorator function or class. Here's an example of a simple decorator that adds a logging statement before and after a function call:

```python

def my_decorator(func):
    def wrapper(*args, **kwargs):
        print("Before the function is called.")
        result = func(*args, **kwargs)
        print("After the function is called.")
        return result
    return wrapper

@my_decorator
def my_function():
    print("Hello, world!")

my_function()
```
In this example, the my_decorator function takes a function func as input, defines a new function wrapper that adds some logging statements, and then returns the wrapper function. The @my_decorator syntax is used to apply the decorator to the my_function function, effectively modifying its behavior by wrapping it with the wrapper function.

When my_function() is called, it first prints "Before the function is called.", then executes the original function code (which prints "Hello, world!"), and finally prints "After the function is called.".
