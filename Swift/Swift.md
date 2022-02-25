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

<br/>

### **Type Annotations**

&nbsp; &nbsp; &nbsp; You can provide a type annotation when you declare a variable, to be clear about the kind of values the variable can store.

**_Syntax_**

```Swift
var variableName:<data type> = <optional initial value>
```

>**Note**: If we are not using _type annotation_, then it becomes mandatory to provide an initial value for the variable


## **Constants**

*Alternative* to the var keyword,if you want to set a value once and never change it.


* Declare with the _**let**_
 
```swift
let pi = 3.141519
```
>**Note**: You can declare multiple _*constants*_ or multiple _*variables*_ on a single line, separated by commas


<br/>

___

<br/>


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

---
## FOR-IN LOOPS
---
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
* ### **Example**
  * For Numeric Ranges

```Swift
for index in 1...5 {
 print("\(index) times 5 is \(index * 5)")
  }
// 1 times 5 is 5
// 2 times 5 is 10
// 3 times 5 is 15
// 4 times 5 is 20
// 5 times 5 is 25

```
**Note:** _You can ignore the values by using an underscore in place of a variable name._

---
## WHILE LOOPS
---
>A while loop performs a set of statements until a condition becomes false.

* are best used when the number of iterations isn’t known before the first iteration begins.

 * Swift Provides Two kinds of While Loops

   * **While** loop evaluates conditions at the start of each pass.

   >_Here’s the general form of a while loop:_
   ```swift
   while condition {
    statements
   }
   ```
  

   * **Repeat** While loop evaluates conditions at the end of each pass.

   > Here’s the general form of a repeat-while 
   loop:
   ```Swift
   repeat {
    statements
    } while condition
    ```




___

