---
description: Structs like c-do.
---

# Structs

Since SMLL targets the JVM, structs are used in-place of classes and they simply map to record classes in java. SMLL doesn't allow mutation of data so all structs are read only and they have no methods. To manupulate structs use functions, like in c.&#x20;

{% code lineNumbers="true" %}
```rust
struct Foo(bar: Int)
struct Person(name: String, age: Int)
```
{% endcode %}

### Struct literals

Structs are useful as long as you can create their instances. Struct instances are just references to the allocated memory used to represent the struct.&#x20;

{% code lineNumbers="true" %}
```sml
val foo = Foo {bar: 20}
val npc = Person {name: "Jake", age: 512} (* Jake is Non playable coz he's dead, lol *)
```
{% endcode %}

