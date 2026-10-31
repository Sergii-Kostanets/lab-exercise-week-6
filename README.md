# Lab Exercise Week 6 - Decisions, Loops and Functions

## Ferry Fare

Open [ferry-fare.html](javascript/ferry-fare.html) in a browser and enter an age when prompted.
The page uses `if` and `else if` statements to show:

- Below 0 or above 120: That is not a valid age
- Under 5: Free
- Under 16: Child fare
- 16 and over: Adult fare

## Why the Order of Conditions Matters

If `else if (age < 5)` is placed after the `if (age < 16)` test, entering age 3 displays "Child fare." The first condition is already true, so the `else if` is never checked. Put the under-5 test first to display "Free" for ages below 5.
