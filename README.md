# C-Day-66-Sum-Divisible-by-5
# C Day 66 - Sum of Numbers Divisible by 5

## Description

This program takes multiple numbers from the user and calculates the sum of all numbers that are divisible by 5.

## Example

```text
Enter how many numbers: 5
Enter number 1: 10
Enter number 2: 12
Enter number 3: 15
Enter number 4: 7
Enter number 5: 20

Sum of numbers divisible by 5 = 45
```

## Code

```c
#include <stdio.h>

int main()
{
    int n, number;
    int sum = 0;

    printf("Enter how many numbers: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++)
    {
        printf("Enter number %d: ", i);
        scanf("%d", &number);

        if (number % 5 == 0)
        {
            sum = sum + number;
        }
    }

    printf("Sum of numbers divisible by 5 = %d", sum);

    return 0;
}
```

## Concepts Used

* `for` loop
* `if` statement
* Modulus operator `%`
* `scanf()`
* Variables
* Addition

## How It Works

1. The user enters how many numbers they want to check.
2. The program takes each number using a `for` loop.
3. The `%` operator checks whether the number is divisible by 5.
4. If the number is divisible by 5, it is added to `sum`.
5. Finally, the program displays the total sum.

## File Name

`sum_divisible_by_5.c`

## Goal

The goal of this program is to practice loops, conditions, the modulus operator, and calculating a sum based on a condition.
