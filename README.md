# Elixir Enum.each List Modification Bug
This example demonstrates a common pitfall when using `Enum.each` in Elixir to modify a list.  Attempting to modify the list directly within the anonymous function does not alter the original list.  The provided solution shows the correct way to achieve the desired outcome.

## Bug
The `bug.exs` file shows an attempt to remove the element `3` from a list during iteration with `Enum.each`. However, this does not work as intended.

## Solution
The `bugSolution.exs` file provides a solution using `Enum.filter` to create a new list without the undesired element.