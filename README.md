# CS50 Cash

## Description

**Cash** is a C program created as part of Harvard's **CS50x** introduction to computer science. The program calculates the minimum number of coins (quarters, dimes, nickels, and pennies) required to give a user a specified amount of change using a greedy algorithm.

---

## How It Works

1. Prompts the user for the amount of change owed.
2. Validates that the input is a non-negative amount.
3. Calculates the minimum number of coins needed by starting with the largest denomination available:

   * **Quarters** ($0.25)
   * **Dimes** ($0.10)
   * **Nickels** ($0.05)
   * **Pennies** ($0.01)
4. Prints the total coin count.

---

## How to Run

1. **Compile the program:**

   ```bash
   make cash
   ```

2. **Run the program:**

   ```bash
   ./cash
   ```

---

## Technologies Used

* **C**
* **CS50 Library**

---

## What I Learned

* Applying a greedy algorithm to solve a practical problem.
* Using loops and conditional statements.
* Validating user input.
* Improving my logical thinking and problem-solving skills.

