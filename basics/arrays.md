---
description: Shoot a ray of arrays
---

# Arrays

Arrays allow us to group together data of the same type into a single access point which is usually a variable. Arrays are indexable by any value of type [Int](types.md), this can be a literal, a function call or an expression. Arrays have bounds in SMLL so it it critical to specify the number of elements the array holds when declaring the array type, but no needed when you specify the array. The compiler counts the elements for you and populates the size of you.  Indexing the arrays has a different form. Use the&#x20;

`.[]` symbol and pass your value inside the brackets.

{% code lineNumbers="true" %}
```sml
val numbers = [1,2,3,4,5,6,7,8,9,10] (* The compiler can deduce the size here*)
fun head(x: [Int; 10]): Int => x.[0] (* Notice how you specified the type of the array *)
```
{% endcode %}

