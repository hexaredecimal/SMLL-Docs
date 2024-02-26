---
description: Like matching outfits
---

# Match

The match expression is inspired by the case expression from **Standard ML**, and th e match expression from **Rust**. The match expression allows you to check if a value is an expected value or type and it can also be used to destructure enums and struct value. More on those later, for now lets match some values. The match expression takes a match value, followed by a list of match cases and their respective bodies to run if they match. The default case is represented by an underscore symbol.

{% code lineNumbers="true" %}
```rust
match 1 + 1 {
    2 -> true
    _ -> false
}
```
{% endcode %}

