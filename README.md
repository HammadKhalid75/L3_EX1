# Kotlin OOP: Employee Salary Calculator

Demonstrates **inheritance**, **polymorphism**, and **collections** in Kotlin.

---

## Classes

| Class | Description |
|------|-------------|
| `Employee` | Base class with `name`, `baseSalary`, and `calculateSalary()` |
| `FullTimeEmployee` | Adds `bonus` → `baseSalary + bonus` |
| `PartTimeEmployee` | Uses `hourlyRate × hoursWorked` |

---

## Key Features

- `open class` and `open fun` for inheritance
- `override` in subclasses
- `mapOf` to store employees
- `forEach` loop with formatted output

---

## Code Highlights

```kotlin
open class Employee(protected val name: String, protected val baseSalary: Double) {
    open fun calculateSalary(): Double = baseSalary
}
