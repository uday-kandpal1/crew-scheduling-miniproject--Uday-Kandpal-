# ✈️ Crew Scheduling & String Matching Algorithms

## 📌 Project Overview

This project implements and analyzes fundamental **algorithm design techniques** through two problem domains:

1. **Crew Scheduling Problem**

   * Solved using **Backtracking** and **Branch & Bound**
   * Focus: Constraint satisfaction and optimization

2. **String Matching Problem**

   * Implemented using **Naive Search** and **KMP Algorithm**
   * Focus: Pattern searching efficiency and performance comparison

The project combines **algorithm implementation**, **conceptual understanding**, and **experimental validation using graphs**.

---

## 🧩 Problem Summary

### 🔹 Tasks 1 & 2: Crew Scheduling

* Assign flights to crew members such that:

  * No overlapping schedules
  * Mandatory **rest time constraint** is satisfied
* Objective:

  * **Minimize the maximum workload** among crew members

#### Techniques Used:

* **Backtracking**

  * Recursively explores all valid assignments
  * Ensures constraints are satisfied at each step

* **Branch & Bound**

  * Optimizes search by pruning suboptimal solutions
  * Avoids unnecessary computation

---

### 🔹 Tasks 3 & 4: String Matching

#### Algorithms:

* **Naive Search**

  * Checks pattern at every index
  * Time Complexity: `O(n * m)`

* **KMP Algorithm**

  * Uses LPS (Longest Prefix Suffix) array
  * Time Complexity: `O(n + m)`

#### Analysis:

* Compare:

  * Execution time
  * Character comparisons
* Visualized using graphs

---

## 🧠 🔹 Task 5: Conceptual Programming Insights

This task highlights the **key algorithmic concepts embedded as inline comments** in Tasks 1–4.

### 📍 Key Concepts from Tasks 1 & 2

* **Backtracking**

  * Explores all possible assignments recursively
  * Uses constraint checking (`is_valid_assignment`) to eliminate invalid paths early

* **Constraint Satisfaction**

  * Ensures:

    * No overlapping flights
    * Mandatory rest time between assignments

* **Branch & Bound**

  * Introduces optimization using a **bounding function**
  * Prunes branches where:

    ```
    potential_load >= current_best_load
    ```
  * Reduces exponential search space significantly

* **Objective Function**

  * Minimizes:

    ```
    maximum workload among all crew members
    ```

---

### 📍 Key Concepts from Tasks 3 & 4

* **Naive String Matching**

  * Brute-force approach
  * Re-checks characters unnecessarily
  * Demonstrates inefficiency for large inputs

* **KMP Optimization**

  * Uses **LPS array** to skip redundant comparisons
  * Avoids re-evaluating known prefixes

* **LPS (Longest Prefix Suffix)**

  * Stores overlap information within pattern
  * Core idea behind KMP efficiency

* **Empirical Analysis**

  * Time complexity measured using `time.perf_counter()`
  * Work complexity approximated via **character comparisons**

* **Graph-Based Validation**

  * Confirms:

    * Naive → grows rapidly (O(n·m))
    * KMP → grows linearly (O(n + m))

---

## ⚙️ Setup Instructions

### 🔧 Requirements

* Python 3.x
* Required library:

  ```bash
  pip install matplotlib
  ```

---

### ▶️ Running the Code

1. Open in:

   * Jupyter Notebook / Google Colab / VS Code

2. Execute in order:

   #### 🟦 Tasks 1 & 2:

   * Crew scheduling implementation
   * Outputs optimal assignment

   #### 🟩 Tasks 3 & 4:

   * String matching algorithms
   * Generates performance graphs

   #### 🧠 Task 5:

   * Review inline comments for conceptual understanding

---

## 📊 Output

### ✅ Crew Scheduling

```
Optimal Maximum Load Achieved: 6 hours
```

---

### 📈 String Matching

* Time Complexity Graph
* Character Comparison Graph

---

## 🧠 Key Learnings

* Backtracking explores **complete search space**
* Branch & Bound improves efficiency via **pruning**
* KMP eliminates redundant work using **pattern preprocessing**
* Graphs validate **theoretical complexity with real data**
* Inline comments reinforce **conceptual clarity**

---


## 👨‍💻 Author

Uday Kandpal
---
