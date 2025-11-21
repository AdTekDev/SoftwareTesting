
# Test 2  

Below is the **English version** of your assignment, rewritten cleanly and academically, following your required structure.

---

# **Assignment — Probability Combination Using Sliding Windows**

You are given a Python function that computes probability distributions of sliding windows of size *n* across multiple arrays. Based on this code, complete the following tasks:

---

## **1. (3.5 points) Design White-Box Test Cases Using Level-7 Coverage**

Design test scenarios using **White-Box testing**, targeting **Level 7 structural coverage**, which may include:

* Statement coverage
* Branch coverage
* Condition coverage
* Loop coverage (zero iteration, one iteration, multiple iterations)
* Path coverage
* Data flow coverage
* Boundary logic reasoning inside the function

Your test design must explicitly reference which internal code paths, branches, and loops each test case is intended to cover.

---

## **2. (2 points) Design Black-Box Test Cases (EP + BVA)**

Design Black-Box test scenarios using at least **two methods**:

* **Equivalence Partitioning (EP)**
* **Boundary Value Analysis (BVA)**

Your test cases should treat the function as a black box, focusing on:

* Valid / invalid partitions
* Minimum and maximum boundary lengths
* Window size constraints
* Input structure constraints

At least **five** Black-Box test cases must be designed.

---

## **3. (1.5 points) Write Python Unit Tests Using Pytest**

Write a Python test file using the **pytest** framework to implement **five unit test cases** based on the function:   

**CODE-01**  
```python
from collections import Counter

def sliding_window_probabilities(arrays, n):
    window_counter = Counter()
    total_windows = 0

    for arr in arrays:
        if len(arr) < n:
            continue
        for i in range(len(arr) - n + 1):
            window = tuple(arr[i:i + n])
            window_counter[window] += 1
            total_windows += 1

    probabilities = {
        window: count / total_windows
        for window, count in window_counter.items()
    }

    return probabilities, window_counter, total_windows
```

Your pytest file must include:

* Setup of input data
* Execution of the function
* Assertions validating the results
* Coverage of at least 5 meaningful test cases

---

## **4. (3 points) Write Python Code in the Lab to Execute All Test Cases**

In the practice lab:

* Write Python code to execute **all designed test cases**, both White-Box and Black-Box.
* **Separate the data from the script**:

  * One file contains test data
  * One file contains the test runner / pytest script

Example structure (you may adapt):

```
/test_data/
    wb_cases.json
    bb_cases.json

/tests/
    test_sliding_window.py
```

Your solution must demonstrate:

* Data-driven testing
* Clear separation between test logic and test data
* Ability to load test data (JSON/CSV/YAML) and run all scenarios programmatically

---

