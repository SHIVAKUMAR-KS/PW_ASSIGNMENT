# Java Array Concepts

This document covers various questions and answers related to arrays in Java. It includes information on array initialization, memory storage, traversal methods, and more.

## Questions and Answers

### 1. What is the default value of an array for different data types?

- **int:** `0`
- **float:** `0.0`
- **double:** `0.0`
- **char:** `'\u0000'`
- **boolean:** `false`
- **Object:** `null`

### 2. Can you pass a negative number in Array size?

No, you cannot pass a negative number as the size of an array. If you try to do so, the Java compiler won't throw an error, but you will receive a `NegativeArraySizeException` at runtime.

### 3. Where is an Array stored in JVM memory?

An array in Java is an object, so it is stored in the heap memory of the JVM.

### 4. What are the disadvantages of an Array?

- **Fixed Size:** The size of an array is fixed at the time of its creation. It cannot be resized dynamically.
- **Contiguous Memory Allocation:** Arrays require contiguous memory space, which might not always be available, leading to memory inefficiency.
- **Static Data Structure:** Arrays are static, meaning their size cannot be altered after creation.

### 5. What is an Anonymous Array in Java? Give an example.

An anonymous array is an array without a name or reference. It's typically used for one-time use cases.

### 6. What are the different ways to traverse an Array in java?

Using for loop 

Using for each loop
###  7. What is the difference between length and length() method

Ans: length
An array is an object that holds a fixed number of values of the

same type.
The length variable in an array returns the length of an array i.e. a

number of elements stored in an

array.
Once arrays are initialized, its length cannot be changed, so the

length variable can directly be used

to get the length of an array.

The length variable is used only for an array.

length()
The length() method is a static method of String class.
The length() returns the length of a string object i.e. the number of

characters stored in an object.

String class uses this method because the length of a string can be

modified using the various operations on

an object.
The String class internally uses a char[] array that it does not

expose to the outside world.

Example:
public class Test {
public static void main(String args[]) {
String str = "Welcome to Tutorials Point";
System.out.println("Length of String using length() method is:
" + str.length());
}
}

Give an Examples?
**Example:**

```java
// Anonymous int array
new int[] {2, 3, 4, 5, 6, 7};

// Anonymous String array
new String[] {"Java", "Hungry"};
