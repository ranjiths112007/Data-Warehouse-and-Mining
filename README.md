# Data Warehousing & Mining 📊

A practical collection of my **Data Warehousing and Data Mining (DWM)** coursework, implemented mainly with Python and NumPy.

This repo focuses on understanding the core ideas by actually implementing them — from multidimensional data analysis and bitmap indexing to association rule mining and external sorting.

## 📚 Tasks & Practical Work

### Task 3 — OLAP Operations with NumPy
`DWM_Task3.ipynb`

Builds a small sales data cube using **Products, Regions and Years** and demonstrates common OLAP operations:

- Slice
- Dice
- Roll-up
- Drill-down
- A reusable `OLAPCube` class for these operations

The notebook works with a `3 × 3 × 2` sales cube and shows the resulting values for each operation.

### Task 4 — Bitmap Indexing
`DWM_Task_4.ipynb`

Implements bitmap indexing for a small student dataset using NumPy bit arrays.

The notebook covers:

- `np.packbits()` and `np.unpackbits()`
- Bitwise **AND**, **OR** and **NOT** queries
- Filtering student IDs using bitmap conditions
- A reusable `BitmapIndexEngine` class

Example queries include **Male AND CSE**, **CSE OR IT**, and **NOT Male**.

### Task 5 — FP-Growth
`task_5.ipynb`

Implements **FP-Growth from scratch** instead of relying on a mining library.

The implementation includes:

- FP-Tree node structure
- FP-Tree construction
- Conditional pattern-base generation
- Recursive FP-Growth
- Support counting for frequent itemsets

The example transaction dataset uses items such as Bread, Milk, Diaper and Beer with a minimum support of `2`.

### Task 6 — External Sorting & Merge Join
`Task_06.ipynb`

Demonstrates how large datasets can be processed when everything cannot simply be sorted in memory.

The notebook covers:

- Generating employee and department CSV datasets
- Splitting data into sorted chunks
- External sorting using a **k-way merge with `heapq`**
- Producing sorted employee and department tables
- Streaming merge-join logic for the sorted data

The example creates **10,000 employee records** and **100 department records** and processes them using chunk-based sorting.

## 🛠️ Tech Stack

**Python · NumPy · Jupyter Notebook · CSV · Heapq · Data Warehousing · Data Mining**

## 📁 Repository Structure

```text
Data-Warehouse-and-Mining/
│
├── DWM_Task3.ipynb       # OLAP cube and operations
├── DWM_Task_4.ipynb      # Bitmap indexing
├── task_5.ipynb          # FP-Growth implementation
├── Task_06.ipynb         # External sorting and merge join
│
├── CMD Screenshot.png    # Practical execution evidence
├── DWM-TASK_2.png        # Task output / evidence
├── VS Code Screenshot.png
│
└── README.md
```

## 🎯 What I’m Learning

The main idea behind this coursework is to move beyond just knowing the definitions.

These tasks helped me work through how data is represented, how multidimensional data can be queried, how indexes can speed up filtering, how frequent patterns can be discovered from transactions, and how large datasets can be processed with limited memory.

## ▶️ Running the Notebooks

Open any `.ipynb` file in **Jupyter Notebook**, **JupyterLab**, **Google Colab**, or **VS Code** and run the cells in order.

Most examples use standard Python and NumPy, so the setup is intentionally lightweight.

## 📝 Note

This repository is part of my **college coursework and practical learning** in Data Warehousing and Data Mining.

---

**Learning the concepts by implementing them, one task at a time.**
