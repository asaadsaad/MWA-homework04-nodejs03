# MWA Homework 4 - NodeJS 03
## Exercise
Create an **HTTP server** that receives a request to the following route: `http://localhost:4000/posts?return=id,title` and is supposed to do an intensive CPU work, this work would block the main event-loop of the master process. 
  
The route would create a child-process and fetch a JSON object from a third-party service `https://jsonplaceholder.typicode.com/posts`, it filters the response of 100 posts based on the query parameters passed to the route, and passes the filtered results back to the main process.  
  
**Example:** if the query params were: `?return=id,title` the response would be JSON with the following structure:
```json
  [{
    "id": 1,
    "title": "doloribus ad provident suscipit at",
  },
  ...]
```
  
**Note:** Node 16.* does not have `fetch()`, you may use the native `http` core module which has `get()` or `request()` methods, or one of the third-party packages like `request`, `axios`, `got`, or `superagent`. 

**Note: Always add `node_modules` folder to your `.gitignore` file. You should only push your code along with `package.json` and `package-lock.json`**

