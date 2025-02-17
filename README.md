# Ruby: Unexpected Immutable Behavior
This example demonstrates a common misunderstanding in Ruby: the lack of implicit setters for instance variables.  If you don't define a `value=` method or use `attr_accessor`, assigning to `object.value` will not modify the object's state.  The solution shows how to correctly define a setter method to enable modification.

## Bug
The `bug.rb` file shows code that attempts to change an object's instance variable without using an explicit setter method.  This results in the value remaining unchanged.

## Solution
The `bugSolution.rb` file shows the corrected code, incorporating a setter method using `attr_accessor` to allow modification of the `@value` instance variable.