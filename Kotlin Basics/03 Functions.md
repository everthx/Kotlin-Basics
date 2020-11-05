# 03 Functions
## Function declarations
Functions in Kotlin are declared using the **fun** keyword:
```kotlin
fun sayHello(){
    println("Hello!")
}
```

## Calling functions
Functions can be called in a very simple way.
```kotlin
val result = sayHello()
```

>### Calling functions from a Class
>Calling member functions can be done with the dot notation:
```kotlin
Person().sayHello() // Where Person() is a class and sayHello a function inside that class
```
>For more information on Classes click [Here]()

## Parameters
Parameters must be explicity declared using Pascal Notation i.e. *name: type* ans separated by commas.
```kotlin
fun getStudent(name: String, year: Int){ /*...*/}
```
>### Default Arguments
>Function parameters can have default values, normaly used to skip an argument.
```kotlin
fun getStudent(name: String, year: Int = 2020){
    println("Got $name from Grad year $year")
}
```
>This can helps us skip the defaults on a function call, *i.e.*
```kotlin
println(getStudent("Joe"))          // OUTPUT: Got Joe from Grad year 2020
println(getStudent("Oscar", 2010))  // OUTPUT: Got Oscar from Grad year 2010
```

## Single-expression functions
When a function returns a single expression, you can remove the curly braces *{}* and specify the body after a **=** symbol:
```kotlin
fun sumTwoNumbers(a: Int, b: Int): Int = a + b
```

## Explicit return types
You can specify the explicit **return** type of a function.
```kotlin
fun isUserUnderage(user: String, age: Int): String{
    return if (age >= 21) "$user is not underage" else "$user is underage"
}
```
