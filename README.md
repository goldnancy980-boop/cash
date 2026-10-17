# Cash

## Project Overview

Cash is a C program I implemented as part of Harvard's CS50 Cash problem set. It calculates the minimum number of coins needed to give a specified amount of change in cents.

The program uses a greedy algorithm to determine the number of quarters, dimes, nickels and pennies required.

## How It Works

1. Prompts the user to enter the amount of change owed in cents.
2. Rejects negative values and requests valid input.
3. Uses the largest possible coin denominations first:

   * Quarters (25 cents)
   * Dimes (10 cents)
   * Nickels (5 cents)
   * Pennies (1 cent)
4. Counts the coins used and prints the total.

## Requirements

* A C compiler
* The CS50 C Library (unless using the alternative approach below)

## How to Get the CS50 Library

This program uses `get_int()` from the CS50 C Library.

**Option 1: CS50 Codespace**

Visit [CS50 Codespace](https://cs50.dev/). The library is available in this environment.

**Option 2: Ubuntu or Debian**

Run these commands in your terminal:

```bash
curl -s https://packagecloud.io/install/repositories/cs50/repo/script.deb.sh | sudo bash
sudo apt install libcs50
```

## How to Compile and Run

Save the program as `cash.c`.

In CS50 Codespace, compile and run it:

```bash
make cash
./cash
```

## Alternative: Without the CS50 Library

You can replace `get_int()` with standard C input using `scanf()` and remove `#include <cs50.h>`. This allows you to run the program without installing the CS50 Library.

Save the modified program as `cash.c`, then compile and run it using:

```bash
gcc cash.c -o cash
./cash
```

**Note:** Unlike `get_int()`, basic `scanf()` input handling may not repeatedly prompt the user after invalid input unless additional validation is implemented.

## Example

**Input:**

```text
Change owed: 41
```

**Output:**

```text
4
```

The program returns `4` because 41 cents requires one quarter, one dime, one nickel and one penny.

## Technologies Used

* C
* CS50 C Library
* Standard C input/output (`stdio.h`)

## What I Learned

* Using loops to repeat operations.
* Validating user input with a `do-while` loop.
* Applying a greedy algorithm to solve a problem.
* Working with the CS50 C Library and standard C input/output.
