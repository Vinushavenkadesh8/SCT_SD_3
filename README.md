# Task 03: Automatic Sudoku Solver 🧩

**Organization:** SkillCraft Technology  
**Domain:** Software Development Internship  
**Task Number:** 03  

---

## 📖 Overview
This project is an automated Sudoku solver built using **Python**. The program takes an input grid representing an unsolved Sudoku puzzle (where `0` represents empty cells) and uses an algorithm to fill in the missing numbers according to the standard rules of Sudoku.

### 📜 Sudoku Rules:
1. Each number (1-9) must appear exactly once in each **row**.
2. Each number (1-9) must appear exactly once in each **column**.
3. Each number (1-9) must appear exactly once in each **3x3 subgrid**.

---

## 🚀 Logic & Algorithm
The solver is implemented using the **Backtracking Algorithm**. This is a recursive approach that:
1.  **Finds** the next empty cell (marked as `0`).
2.  **Attempts** to place a digit from 1 to 9.
3.  **Validates** if the digit follows the rules (no duplicates in row, column, or 3x3 box).
4.  **Recurses:** If valid, it moves to the next cell.
5.  **Backtracks:** If a number leads to no solution, it resets the cell and tries the next possible digit.

### 📈 Complexity Analysis
* **Time Complexity:** $O(9^{n})$, where $n$ is the number of empty cells. 
* **Space Complexity:** $O(n)$ due to the recursion stack.

---

## 🛠️ How to Use
1. **Open the Notebook:** Load the `.ipynb` file in Google Colab or any Jupyter environment.
2. **Input your Grid:** Locate the `grid` variable in the code. Replace the values with your unsolved puzzle (use `0` for empty spots).
3. **Run the Code:** Execute the cells to see the algorithm solve the puzzle in real-time.
4. **View Output:** The program will print the final solved 9x9 grid in the console.

---

## 🖥️ Example Implementation
**Input Grid (Unsolved):**
```python
grid = [
    [5, 3, 0, 0, 7, 0, 0, 0, 0],
    [6, 0, 0, 1, 9, 5, 0, 0, 0],
    [0, 9, 8, 0, 0, 0, 0, 6, 0],
    ...
]
