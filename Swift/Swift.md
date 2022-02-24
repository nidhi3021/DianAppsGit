# **Swift Learning**

## **<span style="color:Thistle">Variables -- Nidhi**</span>

* Variables are place where you can store program data

* They can vary 

* Declare with the _**var**_

```swift
 var str = "Hello"
```
  Because **str** is a variable we can change it:
  ```swift
  str = "Goodbye"
  ```

## **Constants**

*Alternative* to the var keyword,if you want to set a value once and never change it.


* Declare with the _**let**_
 
```swift
let pi = 3.141519
```
>**Note**: You can declare multiple _*constants*_ or multiple variables on a single line, separated by commas

<br/>

___

<br/>

## **Control Flow** -- _Raj_


### _Control flow_ or _flow of control_ is the order function calls, instructions, and statements that are executed or evaluated when a program is running. 
<br/>

> #### Swift provides a variety of control flow statements.
<br/>

* These include **while** loops to perform a task multiple times

* **_if_, _guard_,** and **_switch_** statements to execute different branches of code based on certain conditions

* statements such as **_break_** and **_continue_** to transfer the flow of execution to another point in your code.

<br/>

>Swift also provides a **for-in loop** that makes it easy to iterate over arrays, dictionaries, ranges, strings, and other sequences.

<br/>

> Swift’s **switch** statement is considerably more powerful. 
<br/>

### FOR-IN LOOPS
<br/>

> It is used to iterate over a sequence, such as items in an array, ranges of numbers, or characters in a string.

* ### **Example**
     * _To iterate over an Array_

````swift
let names = ["Anna", "Alex", "Brian", "Jack"]
for name in names {
    print("Hello, \(name)!")
}
// Hello, Anna!
// Hello, Alex!
// Hello, Brian!
// Hello, Jack!
````
> Each item in the dictionary is returned as a **(key, value)** [tuple.](https://www.w3schools.com/python/python_tuples)
* ### **Example**
     * _To iterate over an Dictionary_

 ````swift
let numberOfLegs = ["spider": 8, "ant": 6, "cat": 4]
for (animalName, legCount) in numberOfLegs {
     print("\(animalName)s have \(legCount) legs")
      }
// cats have 4 legs
// ants have 6 legs
// spiders have 8 legs
````
___

## **<span style="color:Thistle">Variables -- Nidhi**</span>
>Variables are place where you can store program data

## **<span style="color:Thistle">Variables -- Nidhi**</span>

* Variables are place where you can store program data

>They can vary 

```swift
 var str = "Hello"
```
  Because **str** is a variable we can change it:
  ```swift
  str = "Goodbye"
  ```

<<<<<<< HEAD
<<<<<<< HEAD
<<<<<<< HEAD

=======
## **Constants**
---
*Alternative* to the var keyword,if you want to set a value once and never change it.


* Declare with the _**let**_
 
```swift
let pi = 3.141519
```
>**Note**: You can declare multiple _*constants*_ or multiple variables on a single line, separated by commas
>>>>>>> 7d54630 (Modified and added description about constants)
=======
>>>>>>> 7000f56 (Revert "Modified and added description about constants")
=======
>>>>>>> 2de7cf1 (Added about Control flow Intro)
