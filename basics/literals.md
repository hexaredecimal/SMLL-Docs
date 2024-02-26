---
description: Literally!
---

# Literals

Small ML Language supports a wide variety of value literals, these are the most basic ones. Complex literals will be introduced later in relevant sections.

### Numbers

SMLL supports two kinds of numbers, integers and float literals. They follow the standard form for numbers which is used everywhere. Numbers have a type associated with them, see below:

{% code lineNumbers="true" %}
```sml
10 (* has type Int *)
0.5 (* has type Double *)
(* Types are discussed in the next section *)
```
{% endcode %}

### Characters

SMLL also supports the character type, also known as char or u8 in other programming languages. As in Java, a character literal is a Unicode-16 char literal.&#x20;



{% code lineNumbers="true" %}
```sml
'a' (* a utf-16 literal *)
'😂' (* An imoji char *)
(* btw characters have type Char 
```
{% endcode %}

### Strings

SMLL supports java strings by default and they are multiline, by default. Strings below to the String type.&#x20;

{% code lineNumbers="true" %}
```sml
"Hello, from a SMLL String!!!" 
"
 This is a multiline
 String in SMLL
"
```
{% endcode %}

### Unit

SMLL also supports the unit literal, inspired by the rust programming language. Unit literals are analogous to void in java, the difference is that they are a value that doesn't represent data. They can be used in place of returning nothing as in void.&#x20;

{% code lineNumbers="true" %}
```sml
() (* Unit literal has type Unit *)
```
{% endcode %}

