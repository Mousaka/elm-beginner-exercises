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
   "Hello Li! Nice to meet you!"
   ```
   1. What happens if you call the greeter with a number instead of a String?
2. Many functions
   1. Write a function that doubles a number
   2. Write a function that adds 3 to a number
   3. Write a function that subtracts 2 from a number
   4. Write a function `manyMaths` that uses the 3 functions implemented in previous steps to:
       * add 3 to a number
       * and then double it
       * and then subtract 2 from it
       - Example: 
         ```
         > manyMaths 4
         12
         ```
   5. Use the pipeoperator `|>` in your function `manyMaths` to reduce parentheses
3. Booleans and If-expressions
    1. Write a function `isEven` that takes a number as input and returns True if the number is even or else False.
    2. Write a function `evenInfoText` that takes a Bool as input and returns either `"The number is even"` or `"The number is not even"`
    3. Write a function `tellMeIfThisIsEven` that checks if a number is even and returns either `"The number is even"` or `"The number is not even"` using the previous two functions
       - Example:
         ```
         > tellMeIfThisIsEven 3
         "The number is no event"
         ```
    4. Use the pipeoperator `|>` in your function `tellMeIfThisIsEven` to reduce parentheses
    5. Create a function `evenSmartInfoText` that **take a number and a Bool** as input and returns either `"The number n is even"` or `"The number n is not even"` where `n` is replaced by the number sent to the function.
    6. Create `tellMeIfThisIsEvenSmart` that works like the function in *iii.* but makes use of `evenSmartInfoText` instead of `evenInfoText`
       - Example:
         ```
         > tellMeIfThisIsEvenSmart 4
         "The number 4 is even"
         ```
