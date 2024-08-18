---
description: A variable number of variables
---

# Variables

A variable is a memory storage used to store a value or a reference. SMLL has two kinds of variable declaration:

{% hint style="info" %}
In SMLL variable are immutable on the language level and can only be modified by the Java block. This is because SMLL tries to follow the "pure functional programming" approach where functions have no side effects. The Java block is a side effect that is allowed by the language.&#x20;
{% endhint %}

### Val

{% code lineNumbers="true" %}
```kotlin
val number = 10
val name = "Jake"
val answer = number * 2
val (op, left, right) = binop (* Value destructuring using val *) 
```
{% endcode %}

The keyword val binds a name, on the left hand side of the expression to a value on the right hand side of the expression. This is similar to how variables work in every other programming language. The val keyword also support value destructuring for struct values.&#x20;

### Let

{% code lineNumbers="true" %}
```ocaml
let 
  number = 10
  name = "Jake"
  answer = number * 2
in answer
```
{% endcode %}

The let keyword binds a list of names to their corresponding expressions and finally returns a result at the end. This is useful of such cases where code readability is sometimes needed:

#### From

{% code lineNumbers="true" %}
```kotlin
val one = 1
val two = 2
val three = 3
val six = one + two + three
```
{% endcode %}

#### To

{% code lineNumbers="true" %}
```kotlin
val six = 
    let
        one = 1
        two = 2
        three = 3
    in one + two + three
    
```
{% endcode %}
