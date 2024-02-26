---
description: Operation success!!
---

# Operators

Operators play a crucial role in computing values in programs and calculations in general. SMLL supports three kinds of operators separated in to two categories, see below:

### Binary operators

#### Math operators

<table><thead><tr><th width="116">Operator</th><th>Description</th></tr></thead><tbody><tr><td>+</td><td>Adding two numeric values</td></tr><tr><td>-</td><td>Subtracting two numeric values</td></tr><tr><td>*</td><td>Multiplying two numeric values</td></tr><tr><td>/</td><td>Dividing two numeric values</td></tr><tr><td>%</td><td>Computing the modulus of two numeric values</td></tr></tbody></table>



#### Logic Operators

{% hint style="info" %}
Logic operators are also know as boolean operators, because they generate values of type **Bool**
{% endhint %}



<table><thead><tr><th width="117">Operator</th><th>Description</th></tr></thead><tbody><tr><td>></td><td>Greater than</td></tr><tr><td>&#x3C;</td><td>Less than</td></tr><tr><td>>=</td><td>Greater or Equals to</td></tr><tr><td>&#x3C;=</td><td>Less of Equals to</td></tr><tr><td>==</td><td>Equal</td></tr><tr><td>!=</td><td>Not equal</td></tr><tr><td>?</td><td>Value if of type</td></tr></tbody></table>



**A Tiny Quirk**

SMLL has a binary operator for checking if a value is of a certain type. The operator takes the following form.&#x20;

{% code lineNumbers="true" %}
```rust
10?Int
```
{% endcode %}



#### Bitwise Operat

#### ors

SMLL supports basic bitwise operators similar to languages like c and rust.&#x20;

<table><thead><tr><th width="119"></th><th></th></tr></thead><tbody><tr><td>>></td><td>Bitwise shift-right</td></tr><tr><td>&#x3C;&#x3C;</td><td>Bitwise shift-left</td></tr><tr><td>&#x26;</td><td>Bitwise and</td></tr><tr><td>|</td><td>Bitwise or</td></tr></tbody></table>

{% hint style="info" %}
Some bitwise operators are explained below, in the unary section
{% endhint %}

### Unary Operator

Unary operators operate on a single value or operand. SMLL supports unary operators from all categories.&#x20;

#### Math operators

<table><thead><tr><th width="123">Operator</th><th>Description</th></tr></thead><tbody><tr><td>| &#x3C;value> |</td><td>Abs operator</td></tr></tbody></table>

#### Logical operators

<table><thead><tr><th width="135">Operator</th><th>Description</th></tr></thead><tbody><tr><td>!</td><td>Logical not</td></tr><tr><td>?</td><td>Is null</td></tr></tbody></table>

#### Bitwise operators

<table><thead><tr><th width="138">Operator</th><th>Description</th></tr></thead><tbody><tr><td>~</td><td>Bitwise not</td></tr></tbody></table>

