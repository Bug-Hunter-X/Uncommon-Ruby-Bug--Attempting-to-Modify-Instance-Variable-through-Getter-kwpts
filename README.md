# Uncommon Ruby Bug: Modifying Instance Variables Through Getters
This repository demonstrates a subtle bug in Ruby related to how instance variables are accessed and modified.

Often, developers new to Ruby (or object-oriented programming in general) might inadvertently try to modify an instance variable through its getter method.  This will not work as expected.

The `bug.rb` file shows this error. The `bugSolution.rb` file offers a solution.

## How to reproduce
1. Clone this repo
2. Run `ruby bug.rb` to see the unexpected behavior.
3. Run `ruby bugSolution.rb` to observe the correct behavior.

## Solution
The solution involves creating a `setter` method (`value=`) to properly modify the instance variable.