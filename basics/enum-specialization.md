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
```kotlin
fun zar(prez: Presidents.Mandela): String => prez + " Was the president of South Africa"
fun usa(prez: Presidents.Mandela): String => prez + " Was the president of America"
fun rus(prez: Presidents.Mandela): String => prez + " Was the president of Russia"
fun dprk(prez: Presidents.Mandela): String => prez + " Was the president of North Korea"
```
{% endcode %}

This is how to use them.&#x20;

{% code lineNumbers="true" %}
```sml
fun main(): Unit => {
    val myprez = Presidents.Mandela
    println(zar(myprez)) (* compiles successfully *)
    println(rus(myprez)) (* fails *)
}
```
{% endcode %}

