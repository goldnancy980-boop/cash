# Cash

## Project Overview

Cash is a C program I implemented as part of Harvard's CS50 Cash problem set. It calculates the minimum number of coins needed to give a specified amount of change in cents using a greedy algorithm.

## How It Works

1. Prompts the user to enter the amount of change owed in cents.
2. Rejects negative values using a `do-while` loop and requests valid input again.
3. Uses the largest coin denominations first:

   * **Quarters:** 25 cents
   * **Dimes:** 10 cents
   * **Nickels:** 5 cents
   * **Pennies:** 1 cent
4. Counts the coins used and prints the minimum total number of coins required.

## Why Use the CS50 Library?

I used `get_int()` from the CS50 C Library (`libcs50`) to simplify user input handling. This allowed me to focus on implementing the greedy algorithm rather than writing input-parsing code from scratch.

## Technologies Used

* C
* CS50 C Library (`libcs50`)
* `stdio.h`
* GNU Make
* GitHub Codespaces
* Dev Containers

## How to Run

### Using GitHub Codespaces

I simplified the development environment using two configuration files:

* **`.devcontainer/devcontainer.json`** — Automates the installation of the CS50 C library when the Codespace is created.
* **`Makefile`** — Defines the compilation settings and required libraries, making it easier to build the program with a single command.

**Steps:**

1. Open this repository on GitHub.

2. Click **Code → Codespaces → Create codespace on main**.

3. Wait for the development environment to finish setting up.

4. Compile the program:

   ```bash
   make cash
   ```

5. Run the program:

   ```bash
   ./cash
   ```

6. Enter the amount of change owed when prompted.

## Example Run

**Input:**

```text
Change owed: 41
```

**Output:**

```text
4
```

**Explanation:** 41 cents requires one quarter, one dime, one nickel and one penny, giving a total of four coins.

## Learning Objectives

* Validating user input using `do-while` loops.
* Implementing a greedy algorithm.
* Working with coin denominations and arithmetic operations.
* Using the CS50 library to simplify input handling.
* Compiling C programs with a Makefile.
* Automating development environment setup with Dev Containers.

