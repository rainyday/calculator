# TDD Tutorial - Python

This tutorial introduces students to Test-Driven Development (TDD) in Python using `unittest`.

## Getting Started

### 1. Install requirements
```bash
pip install -r requirements.txt
```

### 2. Run the tests
```bash
python -m unittest discover -s tests
```

## Workflow

Follow the classic **Red-Green-Refactor** cycle:

1. Write a failing test (`Red`)
2. Write the minimum code to pass the test (`Green`)
3. Refactor for clarity/cleanliness (`Refactor`)

---

## 🧪 Exercise

You will build a simple `calculator` module with the following functions:

- `add(a, b)`
- `subtract(a, b)`
- `multiply(a, b)`
- `divide(a, b)`

Write the test **before** implementing each function.
