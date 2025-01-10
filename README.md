# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: integer overflow in a counter.  The provided VHDL code implements a simple counter, but it lacks proper handling of the upper bound of the integer range. This leads to unexpected behavior when the counter reaches its maximum value.

## Bug Description
The counter increments indefinitely, exceeding the defined range (0 to 15).  This can cause unpredictable results, potentially leading to simulation failures or incorrect hardware behavior.

## Solution
The solution involves adding a modulo operation to wrap the counter back to 0 after reaching the maximum value.  This ensures that the counter operates correctly within its defined range.