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

### **Rules for naming Swift Variables**

1. Variables names must start with either a letter, an underscore `_` , or the dollar sign `$`. For example,
    ```Swift
    // valid
    var a = "hello"
    var _a = "hello"
    var $a = "hello"
     ```

2. Variable names cannot start with numbers. For example,
    ```Swift
    // invalid
    var 1a = "hello" // throws error
    ```

3. Swift is case-sensitive. So `A` and `a` are different variables. For example,
    ```Swift
    var A = 5 
    var a = 55
    print(A) // 5
    print(a) // 55
    ```

4. Avoid using Swift keywords like `var`, &nbsp;`String`, &nbsp;`class`, etc. as variable names.
    
## **Constants**

*Alternative* to the var keyword,if you want to set a value once and never change it.


* Declare with the _**let**_
 
```swift
let pi = 3.141519
```
>**Note**: You can declare multiple _*constants*_ or multiple variables on a single line, separated by commas
<br/>
___

## **Control Flow** -- _Raj_

___

### _Control flow_ or _flow of control_ is the order function calls, instructions, and statements that are executed or evaluated when a program is running. 
<br/>

> #### Swift provides a variety of control flow statements.
<br/>

* These include **while** loops to perform a task multiple times

* **_if, guard,_** and **_switch_** statements to execute different branches of code based on certain conditions

* statements such as **_break_** and **_continue_** to transfer the flow of execution to another point in your code.

<br/>

>Swift also provides a **for-in loop** that makes it easy to iterate over arrays, dictionaries, ranges, strings, and other sequences.

<br/>

> Swift’s **switch** statement is considerably more powerful. 
<br/>

## FOR-IN LOOPS
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

<<<<<<< HEAD
```swift
let numberOfLegs = ["spider": 8, "ant": 6, "cat": 4]
for (animalName, legCount) in numberOfLegs {
    print("\(animalName)s have \(legCount) legs")
          }
// cats have 4 legs
// ants have 6 legs
// spiders have 8 legs
```
=======
     ```swift
     let numberOfLegs = ["spider": 8, "ant": 6, "cat": 4]
      for (animalName, legCount) in numberOfLegs {
        print("\(animalName)s have \(legCount) legs")
          }
    // cats have 4 legs
    // ants have 6 legs
    // spiders have 8 legs
    ```
>>>>>>> 36d657e (Added for Loops)
