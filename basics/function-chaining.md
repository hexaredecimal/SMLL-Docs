---
description: I heard you like chains so I made you one.... with functions.
---

# Function chaining

Function chaining is the ability to continuously evaluate the result of function or computation by appending more functions for the which use the result as input. This simplifies the code and removes the need to set function calls. In SMLL function chaining is supported via the  `.` operator.&#x20;

<pre class="language-sml"><code class="lang-sml">import System::Io

<strong>fn main(): Unit => 
</strong>    let 
        n = 10
    in
        n
            .add(10)
            .sub(5)
            .toString()
            .println()

fn add(x: Int, y: Int): Int => x + y
fn sub(x: Int, y: Int): Int => x - y
fn toString(x: Int): String => x as String

</code></pre>

This works by appending the left side of the `.` operator to the argument list as the first element of the list. The following code

```rust
10
    .add(20)
    .sub(30)
    .mul(3)
    .toString()
    .println()
```

will become

<pre class="language-rust"><code class="lang-rust"><strong>println(toString(mul(sub(add(10, 20), 30), 3)))
</strong></code></pre>

