---
description: Operation success!!
---

# Operators

Operators play a crucial role in computing values in programs and calculations in general. SMLL supports three kinds of operators separated in to two categories, see below:

### Binary operators

### Math operators

<table><thead><tr><th width="116">Operator</th><th>Description</th></tr></thead><tbody><tr><td>+</td><td>Adding two numeric values</td></tr><tr><td>-</td><td>Subtracting two numeric values</td></tr><tr><td>*</td><td>Multiplying two numeric values</td></tr><tr><td>/</td><td>Dividing two numeric values</td></tr><tr><td>%</td><td>Computing the modulus of two numeric values</td></tr></tbody></table>



### Logic Operators

{% hint style="info" %}
Logic operators are also know as boolean operators, because they generate values of type **Bool**
{% endhint %}



<table><thead><tr><th width="117">Operator</th><th>Description</th></tr></thead><tbody><tr><td>></td><td>Greater than</td></tr><tr><td>&#x3C;</td><td>Less than</td></tr><tr><td>>=</td><td>Greater or Equals to</td></tr><tr><td>&#x3C;=</td><td>Less of Equals to</td></tr><tr><td>==</td><td>Equal</td></tr><tr><td>!=</td><td>Not equal</td></tr><tr><td>?</td><td>Value if of type</td></tr></tbody></table>



**A Tiny Quirk**

SMLL has a binary operator for checking if a value is of a certain type. The operator takes the following form.&#x20;

```rust
10?Int
```

