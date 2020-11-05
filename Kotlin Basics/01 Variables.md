# 01 Variables
## val and var
There is 2 basic forms to declare variables, **val** with an unmutable value, meaning once a value is assigned it cannot be changed, and **var** with a mutable value that can change during execution.

>Variables can be asigned a value at declaration or later on the following way:
```kotlin
val a: Int = 1  // You can specify the data type inmediatly when giving a value
val b = 3       // Data type is infered when the value is given
val c: Int      // The data type must be specified if the value is not given
c = 3           // Once c is declared, we can later asign a value to it
```
>This also applies to mutable variables. Mutable variables are declared with **var**
```kotlin
var a: Int = 1
var b = 2
var c: Int
c = a + b
```

## Variable Types
Kotlin, as any other languaje has a wide arange of variable types, here are some of them:
### Integer Numbers
| Type | Size(bits) |
| ----------- | ----------- |
| Byte | 8 |
| Short | 16 |
| Int | 32 |
| Long | 64 |
```kotlin
val oneInt = 1 // Int
val threeBillion = 3000000000 // Long
val oneLong = 1L // Long
val oneByte: Byte = 1
```

### Floating Point Numbers
| Type | Size(bits) | Decimal Digits |
| ----------- | ----------- | ----------- |
| Float | 8 | 6-7 |
| Double | 16 | 15-16 |
```kotlin
val pi = 3.14 // Double
val e = 2.7182818284 // Double
val eFloat = 2.7182818284f // Float, actual value is 2.7182817
```

### Characters
Characters are expressed by the type **Char** and cannot be treated directly as numbers:
```kotlin
val c: Char = 1   // Error: The integer literal does not conform to the expected type Char

val char: Char = '1' // Correct!
```

### Strings
Strings are expressed by the type **String**.
```kotlin
val s: String = "Hello"
val str = "World"
```
You can check other ways of [Working with String Templates](https://github.com/everthx/Kotlin-Basics/blob/main/Kotlin%20Basics/02%20String%20Templates.md).

### Booleans
We can represent **Boolean** variables with one of two values: **true** and **false**

Built-in operations on booleans include:

- **||** - OR
- **&&** - AND
- **!** - Negation
