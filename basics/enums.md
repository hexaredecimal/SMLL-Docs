---
description: Enumerating the enumarators
---

# Enums

Enums help us to describe data that shares a common interface or type but can have different impementations and meaning. They can also be represent data-less types.&#x20;

{% code lineNumbers="true" %}
```rust
enum DaysOfTheWeek = Monday 
    | Tuesday 
    | Wednesday 
    | Thursday 
    | Friday(activit: String) 
    | Saturday
    | Sunday
```
{% endcode %}

This is a enum declaration that represent the days of the week as data-less types, only friday can store data.&#x20;

### Enum literals

{% code lineNumbers="true" %}
```sml
val monday = DaysOfTheWeek.Monday
val friday = DaysOfTheWeek.Friday("Rest")
```
{% endcode %}

