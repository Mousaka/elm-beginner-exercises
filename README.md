# elm-beginner-exercises
# Elm-Lang
## Resources
* http://elm-lang.org - Home page
* http://elm-lang.org/docs - Docs
* https://ellie-app.com - Live code editor
* https://guide.elm-lang.org/install.html - Installation

## Exercises
### Day 1

1. Write a function that takes a String as input and returns a String greeting to that person.
   * Example: 
   ```
   > greeter "Li"
   > "Hello Li! Nice to meet you!"
   ```
   1. What happens if you call the greeter with a number instead of a String?
2. Many functions
   1. Write a function that doubles a number
   2. Write a function that adds 3 to a number
   3. Write a function that subtracts 2 from a number
   4. Write a function `manyMathsOnNumber` that uses the 3 functions implemented in previous steps to:
       * add 3 to a number
       * and then double it
       * and then subtract 2 from it
       - Example: 
         ```
         > manyMathsOnNumber 4
         > 12
         ```
   5. Make use of the pipeoperator `|>` in your function `manyMathsOnNumber`
