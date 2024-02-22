---
description: Instructions on how to install SMLL
---

# Installation

Installing SMLL is a fairly easy process which involves downloading the code and compiling it, then you just use it. Follow the instructions below to complete the installation process.&#x20;

### Prerequisites

* Rust compiler
* JAVA compiler with JDK 21

### Building

```bash
$ git clone depth=1 https://github.com/hexaredecimal/ML.git
$ cd ML
$ cargo build
```

These instructions clone the SMLL repository from github into a folder called ML. Then you change directory (**cd**) to the newly added directory ML. Then build the rust project by calling **cargo build**. This will compile the compiler and place the **smll** binary inside the _target/debug_ directory. Run the following command to check if everything is working.&#x20;

```bash
 $ ./target/debug/smll --help
```

If you see a help file then you are good to go. Lets move on to the next section, Hello world.&#x20;
