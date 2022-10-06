# MWA Homework
## Exercise
Create a web server that may receive a GET request to: `http://localhost:3000?factorial=3` and find the factorial of the passed query-parameter in a seperate child process, the process receives the number as an input, and sends back the factorial of a number as an output. Return the following JSON response: 
```json
{ "factorial": { "input": 3, "output": 6 } }
```
