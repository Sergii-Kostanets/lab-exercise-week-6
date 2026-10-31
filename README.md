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

## Opening Hours Conditions

The shop is closed when the hour is before 9 or is 17 or later. If neither condition is true, the hour must be at least 9 and less than 17, so the shop is open. This is why the `||` check for closed hours gives the same result as checking the open-hours range with `&&`.

## Part 3 - Predict

Puzzles: my predictions (before opening any page)
Puzzle 1: Cool
Puzzle 2: Plenty in stock
Puzzle 3: Silver
Puzzle 4: Bronze
Puzzle 5: Full price
Puzzle 6: Not breezy
Puzzle 7: Take an umbrella
Puzzle 8: Busy
For each wrong prediction: what the page showed, and why:
Puzzle 5: actually showed Discount because I missed second value is true and condition ||.
Puzzle 8: actually showed Busy Open the second door, I missed that second if is a separate decision.

Tickets: what was wrong, and what I changed
Ticket 1: add = to > so it's >= and 16 included.
Ticket 2:
Ticket 3:
Ticket 4:
Validator results: