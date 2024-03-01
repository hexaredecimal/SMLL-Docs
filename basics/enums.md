---
description: Enumerating the enumarators
---

# Enums

Enums help us to describe data that shares a common interface or type but can have different impementations and meaning. They can also be represent data-less types.&#x20;

```rust
enum DaysOfTheWeek = Monday 
    | Tuesday 
    | Wednesday 
    | Thursday 
    | Friday(activit: String) 
    | Saturday
    | Sunday
```

This is a enum declaration that represent the days of the week as data-less types, only friday can store data.&#x20;

### Enum literals

```sml
val monday = DaysOfTheWeek.Monday
val friday = DaysOfTheWeek.Friday("Rest")
```

