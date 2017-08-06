# ti-programs
A collection of TI-BASIC programs I wrote for Texas Instruments calculators.

This collection doesn't contain the more basic scripts I (like many students) wrote to automate formulas and calculations, but rather some of the more interesting programs I wrote as proof-of-concepts.

Here are descriptions of each one:

## List of programs:

### CLOCK

This program displays an analog clock with hour, minute and second hands. The time displayed is taken from the calculator's system time, which can be set under "MODE".

Tested on: TI-84 Plus C Silver Edition

#### Installation:
1. Copy the CLOCK and TIMESAVE programs onto the calculator.
1. Click the "MODE" button, scroll down and ensure the time is set correctly.
1. Run the TIMESAVE program once.
   * TIMESAVE is responsible for syncing the second hand with the minute hand, so that the second hand is at its zero position when the minute hand moves.
   * It may take up to a minute for the program to finish running (it waits for the current minute to change).
   * This program will save a variable "S" in the Archive of the calculator.
1. You can now run CLOCK to display the clock.

### INTSOLVE

This is an discrete/integer numerical equation solver. Given two functions and a prediction value, it will numerically find a solution for the equality of the functions. Unlike the built-in solver, this only considers integer values, which is useful for when your equation contains a function with integer-only inputs (like a discrete probability distribution function).

Tested on: TI-84 Plus Silver Edition and TI-84 Plus C Silver Edition

#### Installation:
1. Copy the INTSOLVE program onto the calculator.
2. Run it, and input two functions, as well as a prediction.
   * Note that if there are multiple solutions, the one that is closer to the prediction will be found.

### SCHEDULE

This is a schedule look-up program for students. When executed, it uses the system time to calculate what class period/block is currently ongoing, which it uses along with an encoded list variable (of the schedule) to determine what class the student should be at then and their next class.

Tested on: TI-84 Plus Silver Edition and TI-84 Plus C Silver Edition

#### Installation:
1. Edit the SCHEDULE program to prepare your own look-up table for classes and their corresponding ID numbers.
1. Copy the SCHEDULE program onto the calculator.
1. Create a list variable (called L6) containing the ID numbers of your classes for each period, with every day from Monday to Friday in consecutive order.
1. Archive the L6 variable.
1. You can now run SCHEDULE to display your current and next classes.
