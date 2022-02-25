# **Swift Learning**

## **<span style="color:Thistle">Variables -- Nidhi**</span>

* Variables are place where you can store program data

* They can vary 

* Declare with the _**var**_ keyword

```swift
 var str = "Hello"
```
  Because **str** is a variable we can change it:
  ```swift
  str = "Goodbye"
  ```

  <br/>

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


<br/>

## **Constants**

A `constant` is a special type of variable whose value cannot be changed.


* Declare with the _**let**_ keyword
 
```swift
let pi = 3.141519
```

Here after `pi` is initialized, we cannot change its value.

>**Note**: You can declare multiple _*constants*_ or multiple _*variables*_ on a single line, separated by commas

<br/>

### **Printing Constants and Variables**
&nbsp; You can print the current value of a constant or variable with the `print` function

```swift
print(str)
//Prints "Goodbye"
```

<br/>

___

<br/>


## **Control Flow** -- _Raj_


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
### **FOR-IN LOOPS**

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
_**Note:**_ _You can ignore the values by using an underscore in place of a variable name._

---
### **WHILE LOOPS**

>A while loop performs a set of statements until a condition becomes false.

* are best used when the number of iterations isn’t known before the first iteration begins.

 * Swift Provides Two kinds of While Loops

   * **While** loop evaluates conditions at the start of each pass.

     - _Here’s the general form of a while loop:_
     <br/>
    
     ```swift
        while condition {
        statements
        }
      ```
  

   * **Repeat** While loop evaluates conditions at the end of each pass.

     - Here’s the general form of a repeat-while loop:
     <br/>

      ```Swift
          repeat {
          statements
          } while condition
      ```

 ## **Conditional Statements**

 Swift provides two ways to add conditional branches to your code: the if statement and the switch statement. 

 
### &nbsp; &nbsp; **IF**
 
 - the if statement has a single if condition. It executes a set of statements only if that condition is true.

   ```swift
   var temperatureInFahrenheit = 30
   if temperatureInFahrenheit <= 32 {
    print("It's very cold. Consider wearing a scarf.")
   }
   // Prints "It's very cold. Consider wearing a scarf."
    ```
- The if statement can provide an alternative set of statements, known as an else clause, for situations when the if condition is false. 
- These statements are indicated by the else keyword.
  ```Swift
   temperatureInFahrenheit = 40
   if temperatureInFahrenheit <= 32 {
    print("It's very cold. Consider wearing a scarf.")
   } else {
    print("It's not that cold. Wear a t-shirt.")
   }
   // Prints "It's not that cold. Wear a t-shirt."
   ```

- You can chain multiple if statements together to consider additional clauses.

  ```Swift
   temperatureInFahrenheit = 90
   if temperatureInFahrenheit <= 32 {
    print("It's very cold. Consider wearing a scarf.")
   } else if temperatureInFahrenheit >= 86 {
    print("It's really warm. Don't forget to wear sunscreen.")
  } else {
    print("It's not that cold. Wear a t-shirt.")
   }
  // Prints "It's really warm. Don't forget to wear sunscreen."
  ```
  _**Note:**_ _The final else clause is optional, however, and can be excluded if the set of conditions doesn’t need to be complete._

  ### **SWITCH**

- A switch statement considers a value and compares it against several possible matching patterns. 
- It then executes an appropriate block of code, based on the first pattern that matches successfully.

     ```Swift 
   switch some value to consider {
   case value 1:
     respond to value 1
   case value 2,
      value 3:
     respond to value 2 or 3
   default:
    otherwise, do something else
   }
    ```






___

