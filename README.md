
# Guided Assignment - Introduction to Conditional Statements in C#

## Introduction

**Conditions in C#:**
Conditions are fundamental to programming as they allow you to control the flow of your program based on certain criteria or expressions. In C#, conditions are used to make decisions in your code. A condition is an expression that evaluates to either true or false.

**`if` Statement:**
The `if` statement is a fundamental control structure in C#. It allows you to execute a block of code if a specified condition is true. Here's how it works:

```csharp
int age = 25;

if (age >= 18)
{
    Console.WriteLine("You are an adult.");
}
```

In this example, we have an `if` statement that checks whether the `age` variable is greater than or equal to 18. If the condition is true, it executes the code inside the curly braces (`{}`) and prints "You are an adult." If the condition is false, the code inside the `if` block is skipped.

**`else if` Statement:**
The `else if` statement is used to provide an alternative condition to be tested if the first `if` condition is false. It's useful when you have multiple conditions to check. Here's how it works:

```csharp
int age = 15;

if (age >= 18)
{
    Console.WriteLine("You are an adult.");
}
else if (age >= 13)
{
    Console.WriteLine("You are a teenager.");
}
else
{
    Console.WriteLine("You are a child.");
}
```

In this example, we first check if the `age` is greater than or equal to 18. If it is, we print "You are an adult." If not, we move to the `else if` condition, which checks if the `age` is greater than or equal to 13. If this condition is true, it prints "You are a teenager." If neither of these conditions is true, the code inside the `else` block is executed, printing "You are a child."

The `else if` statement allows you to provide multiple conditions to handle different cases.

**`else` Statement:**
The `else` statement is used to specify a block of code to be executed if the condition in the preceding `if` or `else if` statement is false. It serves as a fallback or default action. Here's how it works:

```csharp
int age = 8;

if (age >= 18)
{
    Console.WriteLine("You are an adult.");
}
else
{
    Console.WriteLine("You are not an adult.");
}
```

In this example, if the `age` is less than 18, the `else` block is executed, printing "You are not an adult." The `else` statement allows you to handle scenarios where none of the previous conditions are met.

---
## **Requirements:**

1. **Project Setup**:
   - Create a C# Console Project named `GA_Condition_YourName`.
   - Ensure that your name is commented at the top of the program.
   - The project should be structured properly and should run with no compile-time errors.

2. **Implementation of Conditional Statements**:
   - Implement a basic `if` statement as demonstrated in the tutorial.
   - Add an `else` clause to handle cases where the `if` condition is not met.
   - Include an `else if` clause for handling multiple conditions.
   - Modify a variable's value based on the outcome of `if` statements, using a scenario similar to the `temperature` and `weatherInfo` example.

3. **Code Documentation and Style**:
   - Properly comment your code to explain the logic and flow of conditional statements.
   - Follow C# coding conventions for readability and maintainability.

4. **Testing and Validation**:
   - Test your application with various inputs to ensure that all conditional paths are working as expected.
   - Validate that the output is accurate and aligns with the given conditions.

---

## Step By Step

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

### Review The Lecture ( 34:30 - 41:15 )
### https://www.youtube.com/watch?v=QwpnaIsL1MQ&t=2070s

1. **Introduction to Booleans (Time Block: 34:30 - 36:14)**
   - The instructor introduces the concept of Booleans, which represent true or false values in programming.
   - The purpose of Booleans in controlling program flow and making decisions is explained.
   - A simple demonstration of Booleans with the `true` and `false` values is shown.

2. **Introduction to the `if` Statement (Time Block: 36:14 - 39:00)**
   - The `if` statement is introduced as a way to make decisions based on conditions.
   - A basic example of using `if` with the `==` (equality) operator to check if two values are equal is provided.
   - The instructor demonstrates how the `if` statement works with true and false conditions.

3. **Logical Operators (Time Block: 39:00 - 41:15)**
- The concept of logical operators is introduced, and the `==` operator is highlighted.
- The code shows how `==` compares two values for equality.
- The importance of matching data types (e.g., comparing strings in a case-sensitive manner) is emphasized.

Use an if statement to check a condition. For example, checking if a number is equal to 5.

```csharp
static void Main(string[] args)
{
    int number = 5;

    if (number == 5)
    {
        Console.WriteLine("Number is equal to 5");
    }
}
```

**Run your code**  
The message should be printed since 5 is the same as 5.

**Understanding If Statements:** The if statement checks if a condition is true and executes code accordingly.

---

### **Step 2: Adding an Else Clause**

### Review The Lecture ( 41:15 - 45:06 )
### https://youtu.be/QwpnaIsL1MQ?si=bD026-o5A8yw7zIx&t=2475

4. **Using `if` and `else` Statements (Time Block: 41:15 - 45:06)**
   - The `else` statement is introduced as a way to provide alternative code blocks when the `if` condition is not met.
   - A complete example is shown where the user inputs a username, and the code checks if it matches a predefined username.
   - The `if` and `else` blocks are used to display different messages based on the input.

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

### Review The Lecture ( 49:56 - 58:50 )
### https://youtu.be/QwpnaIsL1MQ?si=bD026-o5A8yw7zIx&t=2996

6. **Using `else if` for Multiple Conditions (Time Block: 49:56 - 55:06)**
   - The `else if` statement is introduced as a way to handle multiple conditions in a sequence.
   - A practical example is shown where different user access levels are checked based on their input.
   - The instructor highlights that only one of the `if`, `else if`, or `else` blocks will run based on the first true condition encountered.

7. **Catch-All with `else` (Time Block: 55:06 - 58:50)**
- The `else` statement is explained as a catch-all for conditions that don't match any previous conditions.
- An example demonstrates how the `else` block runs when none of the previous conditions are met.

**Objective:** Learn to use else if for more complex conditions.

Add an else if clause to check for multiple conditions.

```csharp
    if (number == 5)
    {
        Console.WriteLine("Number is 5");
    }
    else if (number == 5)
    {
        Console.WriteLine("Number is greater than 5");
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

### **Step 4: Changing a Variable Based on `if` Statements**

### Review The Lecture ( 45:06 - 49:56 )
### https://youtu.be/QwpnaIsL1MQ?si=bD026-o5A8yw7zIx&t=2706

5. **Variable Scope (Time Block: 45:06 - 49:56)**
   - The concept of variable scope is briefly explained, emphasizing that variables declared within code blocks are only accessible within those blocks.
   - An example demonstrates how changing variable values affects conditional statements.

**Objective:** Learn how to change a variable based on conditions using `if` statements.

In this step, we'll demonstrate how to modify the value of a variable depending on the outcome of `if` statements.

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        int temperature = 75;
        string weatherInfo = "";

        if (temperature > 80)
        {
            weatherInfo = "It's a hot day!";
        }
        else if (temperature > 60)
        {
            weatherInfo = "It's a pleasant day.";
        }
        else
        {
            weatherInfo = "It's a bit chilly.";
        }

        Console.WriteLine(weatherInfo);
    }
}
```

**Explanation:**

1. We have a variable `temperature` representing the current temperature in degrees Fahrenheit and an empty string `weatherInfo` initially.

2. Using a series of `if`, `else if`, and `else` statements, we check the value of `temperature` and update the `weatherInfo` variable accordingly.

3. If the `temperature` is greater than 80, we set `weatherInfo` to "It's a hot day!"

4. If the `temperature` is greater than 60 (but not greater than 80), we set `weatherInfo` to "It's a pleasant day."

5. If none of the above conditions are met (temperature is 60 or lower), we set `weatherInfo` to "It's a bit chilly."

6. Finally, we print out the `weatherInfo` variable to provide a description of the weather based on the temperature.

This example demonstrates how the value of a variable (`weatherInfo`) can be changed based on the conditions specified in the `if` statements.

---

## Rubric:

| Name                                 | Description                                                         | Points   |
|--------------------------------------|---------------------------------------------------------------------|----------|
| Project Setup                        | Correct project creation, naming, and initial setup.                | 20       |
| Basic If Statement                   | Implementation of a basic if statement.                             | 15       |
| If-Else Clause                       | Adding and correctly implementing an else clause.                   | 15       |
| Else If for Multiple Conditions      | Proper use of else if for handling multiple conditions.             | 20       |
| Variable Modification via Conditions | Changing a variable's value based on if statements.                 | 15       |
| Code Documentation and Style         | Clear comments and adherence to coding standards.                   | 10       |
| Testing and Validation               | Comprehensive testing and correct program output.                   | 5        |

**Total Points: 100**

**Additional Notes:**
- Ensure that each step is properly implemented and tested.
- The project should be user-friendly and handle different inputs gracefully.
- Bonus points can be awarded for creativity in implementing additional features or enhancing the user experience.
## Submit your Repo in the textbox on canvas

