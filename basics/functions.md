---
description: What function does that function, function?
---

# Functions

### Functions

SMLL is said to be a functional programming language, that is to say, functions are first-class citizens in this language. Functions can be created, called, stored, passed to functions and returned from other functions. In this section I am just going to introduce the basic usage and creation of functions in SMLL.&#x20;

{% hint style="info" %}
In SMLL all functions have a return type and must always return a value, even unit is a value.oca
{% endhint %}

{% code lineNumbers="true" %}
```swift
fun main(): Unit => {
    val sum = add(20, 50)
    val name = ", the value is" + sum
    greet(name)     
    ()
}

fun add(x: Int, y: Int): Int => x + y
fun greet(name: String): Unit => println("Hello " + name)
```
{% endcode %}

Functions are declared with the fun keyword, followed by a name, arguments and the return type. Then an arrow operator is expected, separating the function header with the body. After the array is a single expression. SMLL functions execute a single expression, even blocks are expressions and blocks can contain more than 1 expressions such that the last one is the return value. Similar to standard compiled programming languages, the entry point of the program is main and functions can be declared anywhere.&#x20;
