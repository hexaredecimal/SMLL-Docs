---
description: Grab it from within
---

# Object Destructuring

Destructuring allows you to access a field of a struct literal, enum expression. This is done using the val keword as follows:

```sml
struct Person(name: String, age: Int)

fun create_greet_message(person: Person): String => {
    val (name, age) = person (* extract the fields *)
    "Hello " + name + " you are " + age + " years old"
}
```
