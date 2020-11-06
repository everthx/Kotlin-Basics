# 04 Classes
## Declaration and instantiation
Classes are declared with the **class** keyword.
```kotlin
class Person
```
You can instantiate a class in a very simple way:
```kotlin
val person = Person()
```
### Properties
Class properties must be explicitly specified:
```kotlin
class Person{
    var name: String = "David"
    var age = 25
}
```
>This will allow that every instance of *Person* has their own *name* and *age*. We could also access and modify these properties for each instance as needed.

## Constructors
