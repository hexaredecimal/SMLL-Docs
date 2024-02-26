---
description: Whats you type?
---

# Types

Static typing is an important concept when it comes to writing reliable software. SMLL is a static typed language, which processes values along with their types to emit the output JAVA program. SMLL has the following built-in types.&#x20;

{% hint style="info" %}
Primitive types are objects in the SMLL backend. They are represented as Java wrapper classes for the primitive types. This is to allow primitive literals such as Int literals to be used as return values from blocks. See the [compiler internals](broken-reference) section&#x20;
{% endhint %}

| Type Name        | Description             |
| ---------------- | ----------------------- |
| Int              | 32 bit integer          |
| Double           | 64 bit float            |
| Float            | 32 bit float            |
| Long             | 64 bit integer          |
| Short            | 16 bit integer          |
| Character        | 16 bit char             |
| String           | A String type           |
| Byte             | 8 bit integer/char      |
| Any              | Polymorphic type        |
| List\[\<type>]   | A Polymophic array type |
| \[\<type>; size] | An array type           |

&#x20;

SMLL also supports structs and enums. These two topics are explained in great detail in their own sections, but for a good impression here they are:

{% code lineNumbers="true" %}
```rust
struct Foo(value: Int) 
```
{% endcode %}

&#x20;This is a basic struct

{% code lineNumbers="true" %}
```rust
enum Option = Some(value: Any) | None
```
{% endcode %}

This is a basic variant enum.&#x20;
