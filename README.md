# Lab Exercise Week 6 - Decisions, Loops and Functions

## Exercise 1

### Ferry Fare

Open [ferry-fare.html](javascript/ferry-fare.html) in a browser and enter an age when prompted.
The page uses `if` and `else if` statements to show:

- Below 0 or above 120: That is not a valid age
- Under 5: Free
- Under 16: Child fare
- 16 and over: Adult fare

### Why the Order of Conditions Matters

If `else if (age < 5)` is placed after the `if (age < 16)` test, entering age 3 displays "Child fare." The first condition is already true, so the `else if` is never checked. Put the under-5 test first to display "Free" for ages below 5.

### Opening Hours Conditions

The shop is closed when the hour is before 9 or is 17 or later. If neither condition is true, the hour must be at least 9 and less than 17, so the shop is open. This is why the `||` check for closed hours gives the same result as checking the open-hours range with `&&`.

### Part 3 - Predict

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
Ticket 2: added && people < 10 to initiate if condition
Ticket 3: combined two separate if desitions into one adding else if instead if
Ticket 4: replace or (||) in the condition to and (&&) so both checks must be true, not only one.
Validator results: all good

## Exercise 2 - Loops

### Part 1 - floors.html

1. Floor 1Floor 2Floor 3Floor 4Floor 5
2. 4, because 5 is not in the scope with < instaed <=.
5. For 5 it's 1, 3, 5. For 6 it's also 1, 3, 5.
6. The Three Parts of a Loop

In the `for` loop `for (var i = 1; i <= 5; i++)`:

- Start: `var i = 1`, which sets the counter's initial value.
- Condition: `i <= 5`, which is checked before each loop iteration.
- Update: `i++`, which increases the counter after each iteration.

In the `while` loop in `floors.html`:

- Start: `var i = 1`, written before the loop.
- Condition: `i <= lastFloor`, in the `while` statement and checked before each iteration.
- Update: `i++`, written inside the loop body so the counter increases after each floor is written.

### Part 2 - times-table.html

1 x 7 = 7
10 x 7 = 70

### Part 3 - reading-room.html

3. 4 times. The door stays locked.
4. 3 times.

Puzzles: my predictions (before opening any page)
Puzzle 1: 123
Puzzle 2: 012
Puzzle 3: 123
Puzzle 4: 10
Puzzle 5: 
1
2
3
Puzzle 6: 1 2 3 
Puzzle 7: 123
Puzzle 8: 4
For each wrong prediction: what the page showed, and why:
Puzzle 3: *** - I missed that document.write returns a star, not a variable.
Puzzle 7: 12 - I missed that break stoppes for loop from if decision.

Tickets: what was wrong, and what I changed
Ticket 1: add  + "<br>" to document.write output.
Ticket 2: add = to < so it's <= to include 6.
Ticket 3: add break after message = "The gate opens"; to exit loop.
Ticket 4: remove quotes around i to output value instaed of the string / char "i".
Validator results: no errors.

## Exercise 3 - Functions

### Part 1 - lamp.html

What the page showed when the function was written but never called: we never called a function, so page shows only the heading.
What happened to the heading and the button when I clicked with document.write in the function: heading and button dissapeared because document.write run after page loaded and rewrite the whole page.
What was different with alert: all elements stayed on their places, alert adds on top.

### Part 2 - visitor-tally.html

What Show visitors said after Add visitor four times: 4
What it said after I reloaded the page, and why: 0. Reloading runs the script again from the top, so the count starts again at zero. 

### Part 3 - Predict

Puzzles: my predictions (before opening any page)
Puzzle 1: no output from fuction as it's not called.
Puzzle 2: Hi!Hi!
Puzzle 3: no output as there are no brackets after function name when trying to call it.
Puzzle 4: 10
Puzzle 5: BAB
Puzzle 6 (the two pop-ups): 2 and 3
Puzzle 7: Note saved (headin and button dissapeared)
Puzzle 8: 0
For each wrong prediction: what the page showed, and why:
all correctly predicted.

Tickets: what was wrong, and what I changed
Ticket 1: add welcome(); after fuction declaration to call it.
Ticket 2: add brackets after function name to call it correctly.
Ticket 3: replace document.write with alerts to save the initial page elements.
Ticket 4: replace line stamps + 1; with stamps = stamps + 1; to correctly save value in the variable.
Validator results: no errors.

## Exercise 4 notes: Function values

### Part 1 - turf.html

In my own words: a parameter and an argument: parameter is a variable fuction awaits, argument is a variable function gets.
What the page showed when getArea returned a value and nothing used it, and why: we didnt assign returned value to a variable.
- width and height are parameters.
- lawnWidth is an argument (variable passed to the function).
- 4 is a value stored in a variable or passed directly.

### Part 2 - delivery.html

What the page showed for 49 and for 50: $4.00 for 49 and $0.00 for 50.
The three things that happen to the order total, from the prompt to the page:
1. `prompt` asks for the order total, and `Number` converts the entered text to a number.
2. The number is passed as the `orderTotal` argument to `getDeliveryCost`. The function checks whether it is at least 50 and returns 0 if it is, or 4 otherwise.
3. The returned delivery cost is formatted to two decimal places with `toFixed(2)`, added to the output text, and displayed with `document.write`.

Puzzles: my predictions (before opening any page)
Puzzle 1: 8 after heading
Puzzle 2: 5 after heading
Puzzle 3: 23 after heading
Puzzle 4: Done after heading
Puzzle 5: B after heading
Puzzle 6: after heading:
6
-6
Puzzle 7: 25 in alert
Puzzle 8: Hot Mild - after heading
For each wrong prediction: what the page showed, and why:
Puzzle 5: A, because return "A"; immediately ends the function and returns "A". document.write("B"); is unreachable.

Tickets: what was wrong, and what I changed
Ticket 1:
Ticket 2:
Ticket 3:
Ticket 4:
Validator results:
