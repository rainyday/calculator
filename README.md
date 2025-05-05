# TDD Worksheet – Calculator Case (Python)

This worksheet will guide you through the process of applying **Test-Driven Development (TDD)** to build a simple calculator in Python. You will follow the classic **Red-Green-Refactor** cycle for each arithmetic operation.

---


## Case Description

You are asked to build a `Calculator` module that supports the following operations:
- Addition (`add`)
- Subtraction (`subtract`)
- Multiplication (`multiply`)
- Division (`divide`)

All operations must be **covered by test cases first**, before the actual implementation.

---

## Project Setup

Your project should have the following structure:

```
tdd_calculator/
├── calculator/
│   └── operations.py
├── tests/
│   └── test_operations.py
```

Make sure you can run tests using the following command:

```bash
python -m unittest discover -s tests
```

---

## Step-by-Step Instructions

### 1. Write a Test for `add()` – Red Phase

In `tests/test_operations.py`, write a test case for the addition function:

```python
import unittest
from calculator.operations import add

class TestCalculator(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(2, 3), 5)
        self.assertEqual(add(-1, 1), 0)
        self.assertEqual(add(0, 0), 0)

if __name__ == '__main__':
    unittest.main()
```

Run the test, and confirm it **fails** because the function does not exist yet.

---

### 2. Implement `add()` – Green Phase

In `calculator/operations.py`, implement the `add()` function:

```python
def add(a, b):
    return a + b
```

Run the test again. It should now **pass**.

---

### 3. Continue the Cycle for Other Operators

Now repeat the Red-Green-Refactor cycle for the following:

- `subtract(a, b)` → with test case and implementation
- `multiply(a, b)` → with test case and implementation
- `divide(a, b)` → make sure to test division by zero (expect an exception)

Write each test first, make sure it fails, then write the implementation.

---

💡 **Extra Challenge!**  
If this calculator case feels too easy for you, maybe basic math is already beneath your greatness.  
Feel free to level up with the **TDD Bus Fare** repo – where real-world logic and chaos await.  
👉 [Go to the Bus Fare repo](https://github.com/alfhisa/tutorial-tdd-bus-fare)

