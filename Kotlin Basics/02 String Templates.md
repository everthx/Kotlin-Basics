# 02 Working with Strings and String Templates
## Strings
You can concatenate strings using the **+** operator. You can also concatenate strings with values of other types, as long as the first element in the expression is a string:
```kotlin
val s: String = "Hello " + 1
print(s + " World")
// OUTPUT: Hello 1 World
```

### Scaped Strings
Scaping string are traditional donde with a backslash. Supported scape sequence are:\n, \t, \b, \r, \', \\, \$
```kotlin
val s = "Hello World!\n"
```
### Raw Strings
A raw string is delimited by a triple quote ("""), it has no scaping and can contain newlines and other characters:
```kotlin
val text = """
    for (c in "foo")
        print(c)
"""
```

## String Templates
String templates can be used on pieces of code that are evaluated and whose results are concatenated into the string. A template expression starts with a dollar sign **$**:
```kotlin
val i = 10
println("i = $i")
// OUTPUT: i = 10
```
or an arbitrary in curly braces:
```kotlin
val s = "abc"
println("$s.length is ${s.length}")
// OUTPUT: abc.length is 3
```
