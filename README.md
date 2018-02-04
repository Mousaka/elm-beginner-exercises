# elm-beginner-exercises
# Elm-Lang
## Resources
* http://elm-lang.org - Home page
* http://elm-lang.org/docs - Docs
* https://ellie-app.com - Live code editor
* https://guide.elm-lang.org/install.html - Installation

## Exercises
### Session 1 functions

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
4. [Case Of](http://elm-lang.org/docs/syntax#conditionals)
   1. Solve by using the case-expression: Create a function that takes a number and returns "One" if the number is 1, "Two" if 2, etc, up to 5. If the number is bigger than five return "Too big!"
### Session 2 Lists

1. Combine two lists together.
2. Create a function that returns the first element of a list
3. Create a function that returns the last element of a list
4. Function on elements
   1. Create a function that adds 1 to each number to a list of numbers.
       - Example:
         ```
         > add1ToAll [1, 2, 3]
         [2, 3, 4]
         ```
   2. Create a function applies the function created in *Session 1 4.i* to each number in the list, resulting in a list of strings.
      - Example:
        ```
        > textifyNumbers [1, 2, 6]
        ["One", "Two", "Too big!"]
        ```
   3. Create a function that takes a function and a list and then applies the function to each element.
 5. Solve *4.i & 4.ii* using [List.map](http://package.elm-lang.org/packages/elm-lang/core/5.1.1/List#map)
 6. Filter lists
    1. Create a function that takes a list of numbers and filters out all the uneven numbers, returning only the even numbers in a list.
       - Example
         ```
         > onlyEven [1, 2, 3, 4]
         [2, 4]
         ```
    2. Create a function that takes a list of strings and removes every string equal to "Too big!" and returns remaining elements in a list.
    3. Create a function that takes a predicate (function taking an element and returns Bool) and a list och elements. The function will try the predicate on every element and filter out all elements that made the predicate return False.
7. Solve *6.i & 6.ii* by using [List.filter](http://package.elm-lang.org/packages/elm-lang/core/5.1.1/List#filter)
