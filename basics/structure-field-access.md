---
description: The need for field access
---

# Structure field Access

Defining data structures is important for writing efficient and maintainable software. Without the ability to access and use the data stored structures become a redundant feature. In SMLL data structure fields can be extracted from instances either using [Object Destructuring](object-destructuring.md) or using the `::` operator.&#x20;

```rust
struct Foo (bar: Int)

fn main(): Unit => 
    let
        baz = Foo {bar: 200}
    in printf("Bar = %d\n", baz::bar) 
```

This allows the users to write concise code that that is re-usable as structs can be composed to form even more complex data structures. &#x20;
