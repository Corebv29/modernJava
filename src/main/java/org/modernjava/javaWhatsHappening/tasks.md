🎯 Study Card Breakdown: Java 8–11 Features
🔍 1. Core Learning and Exploration
✅ Understand Lambda Expressions

Learn the syntax of lambda expressions

Compare lambdas with anonymous inner classes

    Try lambda usage with Comparator, Runnable, and event listeners

✅ Work with the Stream API

Understand what streams are and why they're useful

Explore intermediate operations: filter(), map(), sorted()

    Use terminal operations: forEach(), collect(), reduce()

✅ Master the Optional class

Learn to create Optionals (Optional.of(), .empty(), .ofNullable())

Safely retrieve values using .get(), .orElse(), .ifPresent()

    Replace null checks in old code with Optional

✅ Use the New Date/Time API (java.time)

Understand LocalDate, LocalTime, LocalDateTime

Practice date arithmetic and formatting

    Convert from legacy Date and Calendar to java.time

✅ Explore Java 9–11 Enhancements

Learn about the Java Platform Module System (JPMS)

Use var for local variable type inference (Java 10)

Learn about new methods on collections (List.of(), etc.)

    Understand local-variable syntax for lambda parameters (Java 11)

🧠 2. Practice and Application
✅ Mini Exercises

Write a small lambda to sort a list of strings by length

Use Stream API to filter a list of integers for values > 5

    Convert a nullable return value into an Optional and handle it

💻 3. Coding Challenge — Stream Processing
Steps:

Create a list of integers 1–10

Use .stream() on the list

Apply .filter(n -> n % 2 == 0)

Chain with .map(n -> n * n)

Finish with .reduce(0, Integer::sum)

    Print the result

Expected Output:

Sum of squares of even numbers: 220

📚 4. Dive Deeper (Optional Resources)

Read Chapters 6 & 7 in "Effective Java" (Covers lambdas and Optionals)

Skim through "Java 9 Modularity" to understand JPMS

Convert this code to new java versions (lambda, streams, etc)
```
public static List<Apple> filterGreenApples(List<Apple> inventory) {
    List<Apple> result = new ArrayList<>();                           1
    for (Apple apple: inventory){
        if (GREEN.equals(apple.getColor())) {                         2
            result.add(apple);
        }
    }
    return result;
}


public static List<Apple> filterHeavyApples(List<Apple> inventory) {
    List<Apple> result = new ArrayList<>();
    for (Apple apple: inventory){
        if (apple.getWeight() > 150) {                1
            result.add(apple);
        }
    }
    return result;
}
```