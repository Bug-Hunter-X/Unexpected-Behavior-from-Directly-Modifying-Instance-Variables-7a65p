# Ruby Bug: Instance Variable Side Effects

This repository demonstrates a common, yet subtle, bug in Ruby: directly modifying instance variables using `instance_variable_set` without proper encapsulation. This can lead to unexpected behavior and make code difficult to maintain.

The `bug.rb` file shows an example where an instance variable is manipulated directly, bypassing any potential validation or logic within the class's methods.  The `bugSolution.rb` file presents a more robust solution.

## How to Reproduce

1. Clone this repository.
2. Run `ruby bug.rb` to observe the unexpected output.
3. Run `ruby bugSolution.rb` to see the improved, more maintainable approach.

## Solution

The best practice is to always access and modify instance variables through methods, allowing for better encapsulation and control.