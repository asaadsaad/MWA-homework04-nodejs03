# MWA Homework 4 - NodeJS 03
## Exercise
Create an **HTTP server** that receives a request to the following route: `http://localhost:4000/posts?filterBy=id,title` and is supposed to do an intense CPU work, this work would block the main event-loop of the master process. 
  
The route would start a child-process and fetch a JSON object from a third-party service `https://jsonplaceholder.typicode.com/posts`, it filters the response of 100 posts based on the query parameters passed to the route, and passes the filtered results back to the main process.  
  
The previous route returns a JSON object with the following structure:
```json
  [{
    "id": 1,
    "title": "doloribus ad provident suscipit at",
  },
  ...]
```
  
**Note:** Node does not have `fetch()` in the current stable release, you may use the native `http` core module which has `get()` or `request()` methods, or one of the third-party packages like `request`, `axios`, `got`, or `superagent`. 

**Note: Add `node_modules` folder to your `.gitignore` file. You should only push your code along with `package.json` and `package-lock.json`**

