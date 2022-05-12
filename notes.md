# Agenda

- managing complexity
- local complexity
- The axis of evil
- feature complexity
- the four elements of progamming
- application complexity
- the fifth element of programming
- distributed complexity

https://github.com/onehungrymind/fem-enterprise-patterns

# Why its called enterprise patterns

- solve complexity with the dilligent application of first principles
  - understand why an initiative failed
  - change the way people thing and it will change how they code
  - hardest thing in programming is managing complexity in code
  - the biggest problem in the development and maintenance of large systems is complexity
    - one of the most complex things is the mangement of state and flow of control
    - iron triangle of programming: handling of state - code volume - flow of control
    - no yolo commits

# Complexity

- shared mutable state is dangerous
- leads to coupling of components
- what are the alternatives?
  - ...
- micro complexity
  - a method and what it does
- mezo (in between) complexity
  - components or libs (intra component communication)
- macro complexity
  - application or application(s) level

## The Axis of Evil

- it is impossible to write good tests for bad code
  - if tests are hard to write, code is problematic
- Sub items of the Axis of Evil
  - hidden state
  - violating single purpose function principle
    - a "single purpose" can be coordination and delegation to other functions. Tests of coordination or ATC functions should test the delegation not necessarily the every in/out result
  - nested logic
- Solutions to these
  - dependency injection
  - extract a method
- Can you over divide into smaller and smaller functions?
  - yes, find the team sweet spot and avoid coupling
