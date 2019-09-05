# MWA Homework 4 - NodeJS 03
## Exercise
Create a **Reactive HTTP server** that receives a number passed in the request as query parameter as following: `http://localhost:4000/?n=10` and returns the Fibonacci number of `n`.  
**Example**: `?n=10` should return a `JSON` object: `{fib: 55}`  
  
**Note:** Calculating Fibonacci is considered an intense CPU work, design your code so you don't block the main event-loop while Fibonacci is being calculated in `V8` JS Engine of the master process. 
