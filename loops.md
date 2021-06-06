# Operators and Loops
  lest start with **operators**
  Operators

JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

   - Assignment operators
   - Comparison operators
  - Arithmetic operators
  - Bitwise operators
  - Logical operators
  - String operators
  - Conditional (ternary) operator
  - Comma operator
  - Unary operators
  - Relational operators

### JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator. A binary operator requires two operands, one before the operator and one after the operator: 
  > [click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#assignment_operators) for each operator info .

  # Loops and iteration 
  - Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript.

- You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:

`for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}`

- There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. (Note that it's possible that number could be zero!)

The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.

The statements for loops provided in JavaScript are:

- for statement
-  do...while statement
-   while statement
-   labeled statement
-   break statement
-   continue statement
-   for...in statement
-   for...of statement

> [click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
to know more abot them.

- ** we will focus on for and while  loop** 
## for statement

- A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

- A for statement looks as follows:

- for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement

- When a for loop executes, the following occurs:


  The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
   The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely the condition is assumed to be true.)
  The statement executes. To execute multiple statements, use a block statement ({ ...}) to group those statements.
  If present, the update expression incrementExpression is executed.
   Control returns to Step 2.
### [Example](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration#example)


## while statement

- A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

- while (condition)
  statement

- If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

- The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

- To execute multiple statements, use a block statement ({ ... }) to group those statements.
[Example](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration#example_2)