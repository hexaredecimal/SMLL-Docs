---
description: You are special, like the enum types
---

# Enum Specialization

Each branch or instance of the enum can also be used to represent the specific type. This allows us to write straight forward functions which expect a specific value of the enum. This approach eliminates the over-use of the match expression as a way to decide datatypes inside a function.&#x20;

{% code lineNumbers="true" %}
```rust
enum Presidents = Mandela | Obama | Putin | JunPing
```
{% endcode %}

We can write the specialization functions like this.&#x20;

{% code lineNumbers="true" %}
```rust
fn zar(prez: Presidents.Mandela): String => prez + " Was the president of South Africa"

```
{% endcode %}

This is how to use them.&#x20;

{% code lineNumbers="true" %}
```sml
fn main(): Unit => {
    val myprez = Presidents.Mandela
    println(zar(myprez)) (* compiles successfully *)
    println(rus(myprez)) (* fails *)
}
```
{% endcode %}

