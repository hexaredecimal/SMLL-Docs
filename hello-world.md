---
description: A humble greeting from SMLL
---

# Hello World

Well you are here! That means you now have the smll compiler working on your system and now we are going to write and compile a simple "hello world" program to demonstrate how the language mostly looks like.&#x20;

{% code title="hello.smll" overflow="wrap" lineNumbers="true" %}
```csharp
using System::Io

fun main(): Unit => println("Hello, world")
```
{% endcode %}

Here we are doing the following:

{% code lineNumbers="true" %}
```csharp
using System::Io
```
{% endcode %}

This imports code definitions from the Io module in the System namespace. More on namespaces and modulesI

{% code lineNumbers="true" %}
```csharp
fun main(): Unit => println("Hello, world")
```
{% endcode %}

This defines a function called main which receives zero arguments and returns Unit. Unit is a type similar to **void** in JAVA, more on type on the coming sections. The arrow operator is used to separate the function header from the body expression. In smll functions only have one expression as the body. In this case we simply call the function println with the argument "Hello, world" passed as input to the function. The println function is imported from the Io module, remember? The println function also returns unit so the return value gets promoted to the return of main.&#x20;



### Compile it

To compile run the following command.

{% hint style="info" %}
Before compiling smll expects a build directory to be present in the root directory of your project. If you have created a build folder run the following command to do so.&#x20;
{% endhint %}

{% code lineNumbers="true" %}
```bash
$ mkdir build
```
{% endcode %}

This is going to be replaced by a compiler command argument for creating a project structure.

{% code lineNumbers="true" %}
```bash
./target/debug/smll hello.sml
```
{% endcode %}

You should then get the following output

{% code lineNumbers="true" %}
```bash
Writing ir to file: `Hello.java`
process exited with status: exit status: 0 
```
{% endcode %}

The exit status is from the java compiler process which just compiled the output file "Hello.java"

### Run it!

To run the compiled program use the java compiler like so.&#x20;

{% code lineNumbers="true" %}
```java
java --enable-preview --source 21 Hello.java  
```
{% endcode %}

or pass an extra command line argument like --run to automatically invoke the java compiler for you and run your code.&#x20;

{% code lineNumbers="true" %}
```csharp
/target/debug/smll --run hello.sml
```
{% endcode %}

&#x20;
