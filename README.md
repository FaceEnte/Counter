# Counter Exercise

This project demonstrates the implementation of a simple counter in Java. The exercise involves creating two classes: `CounterTest` and `Counter`. Below are the detailed steps and requirements to complete the exercise.

---

## Objective
Implement a counter with methods to increment its value, reset it, and retrieve its current value. The counter is tested using a provided test program.

---

## Steps to Complete

### 1. Create a New Java Project
- Open **Eclipse**.
- Create a new Java project named `Counter`.

### 2. Create the `CounterTest` Class
- Inside the project, create a new class named `CounterTest`.
- Implement the following test program in the `main` method of the class:

```java
public class CounterTest {
    public static void main(String[] args) {
        Counter counter = new Counter();
        System.out.println(counter.getValue() + ", expected 0");
        counter.countUp();
        counter.countUp();
        System.out.println(counter.getValue() + ", expected 2");
        counter.reset();
        System.out.println(counter.getValue() + ", expected 0");
    }
}
```

### 3. Create the `Counter` Class
- Inside the same project, create another class named `Counter`.
- Implement the `Counter` class with the following:
    - **Instance Variable:**
        - `private int value;`
            - Stores the current value of the counter.
    - **Constructor:**
        - Initialize `value` to `0` when a new `Counter` object is created.
    - **Public Methods:**
        - `int getValue()`:
            - Returns the current value of the counter.
        - `void countUp()`:
            - Increments the value of the counter by 1.
        - `void reset()`:
            - Resets the value of the counter to `0`.

### 4. Expected Output
When you run the `CounterTest` program, the output should be:

```
0, expected 0
2, expected 2
0, expected 0
```

---

## Example Implementation

### Counter Class:
```java
public class Counter {
    private int value;

    // Constructor
    public Counter() {
        value = 0;
    }

    // Method to get the current value
    public int getValue() {
        return value;
    }

    // Method to increment the counter
    public void countUp() {
        value++;
    }

    // Method to reset the counter
    public void reset() {
        value = 0;
    }
}
```

### CounterTest Class:
```java
public class CounterTest {
    public static void main(String[] args) {
        Counter counter = new Counter();
        System.out.println(counter.getValue() + ", expected 0");
        counter.countUp();
        counter.countUp();
        System.out.println(counter.getValue() + ", expected 2");
        counter.reset();
        System.out.println(counter.getValue() + ", expected 0");
    }
}
```

---

## Notes
- Ensure the `CounterTest` and `Counter` classes are in the same package or adjust the package declarations as needed.
- Test the implementation by running the `CounterTest` class.

Happy coding! 🎉
