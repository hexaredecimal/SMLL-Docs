---
description: Modular, like the 80s
---

# Modules

Modules are important because they allow us to store and structure code as folders in the filesystem. They are mostly useful fo sparating different implementations of data and functions. SMLL moduls are inspired by Java Packages. They are just nested folders.&#x20;

{% code lineNumbers="true" %}
```csharp
using System::Io
```
{% endcode %}

Some where there is a modules path which the standard library is located. Inside that modules directory there is a directory named System with the Io file.&#x20;

```bash
<ROOTDIR> 
    └─ System 
        └─── Io.sml
        └─── Result.sml
        └─── Io
             └─── StdIo.sml
```

Importing modules simply works like this.&#x20;

{% code lineNumbers="true" %}
```csharp
using System::Io::Stdio
using System::Io
using System::Result
```
{% endcode %}

These simply translate to the following.&#x20;

{% code lineNumbers="true" %}
```bash
imports System/Io/Stdio.sml
imports System/Io.sml
imports System/Result.sml
```
{% endcode %}
