
# Guided Assignment - Introduction to Conditional Statements in C#

## Tutorials

### Starting Code
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Checking Conditions");
    }
}
```

**Understanding the Code:** This code is the starting point for our exploration of conditional statements in C#. We will modify it to learn how to make decisions in code.

**Write this code**  
- Add a comment above the `Main` method to give context.

```csharp
    // Entry point of our C# program
    static void Main(string[] args)
    {
        Console.WriteLine("Checking Conditions");
    }
```

---

### **Step 1: Basic If Statement**

**Objective:** Learn to use a simple if statement.

Use an if statement to check a condition. For example, checking if a number is greater than 5.

```csharp
static void Main(string[] args)
{
    int number = 10;

    if (number > 5)
    {
        Console.WriteLine("Number is greater than 5");
    }
}
```

**Run your code**  
The message should be printed since 10 is greater than 5.

**Understanding If Statements:** The if statement checks if a condition is true and executes code accordingly.

---

### **Step 2: Adding an Else Clause**

**Objective:** Learn to use an else clause with an if statement.

Add an else clause to handle the case where the condition is not true.

```csharp
    if (number > 5)
    {
        Console.WriteLine("Number is greater than 5");
    }
    else
    {
        Console.WriteLine("Number is not greater than 5");
    }
```

**Run your code**  
Try changing the value of `number` and see how the output changes.

**Understanding Else Clause:** The else clause is executed when the if statement's condition is false.

---

### **Step 3: Else If for Multiple Conditions**

**Objective:** Learn to use else if for more complex conditions.

Add an else if clause to check for multiple conditions.

```csharp
    if (number > 5)
    {
        Console.WriteLine("Number is greater than 5");
    }
    else if (number == 5)
    {
        Console.WriteLine("Number is 5");
    }
    else
    {
        Console.WriteLine("Number is less than 5");
    }
```

**Run your code**  
Modify `number` to test different conditions.

**Understanding Else If:** The else if allows you to check additional conditions if the previous ones were false.

---

### **Step 4: Using Logical Operators**

**Objective:** Introduce logical operators in conditions.

Use logical operators like `&&` (AND) and `||` (OR) in conditions.

```csharp
    if (number > 5 && number < 10)
    {
        Console.WriteLine("Number is greater than 5 and less than 10");
    }
```

**Run The Code**

Change `number` to test the condition.

**Understanding Logical Operators:** Logical operators allow combining multiple conditions in a single if statement.

---

### **Step 5: Nested If Statements**

**Objective:** Understand nested if statements.

Write an if statement inside another if statement.

```csharp
    if (number > 0)
    {
        if (number % 2 == 0)
        {
            Console.WriteLine("Number is positive and even");
        }
    }
```

**Run your code**

Test with different numbers to see how nested conditions work.

**Understanding Nested If Statements:** Nested if statements allow for checking conditions within conditions, creating more complex logic flows.

---

### Additional Tips and Resources

- **Debugging:** Check for syntax errors and ensure conditions are correctly formed.
- **Challenge:** Create a condition that checks whether a number is positive, negative, or zero, and whether it's even or odd.
- **Further Learning:** Dive deeper into conditional logic by exploring switch statements and ternary operators.
- **Syntax Highlighting:** Notice how the different conditional keywords are highlighted if you are reading this online.

---
