# MWA Homework 4 - NodeJS 03
## Exercise 01
Create a Reactive HTTP server that serves simple `.txt` files, where the filename is passed in the request as query parameter.  
The file path is provided in the URL like this: `http://localhost:4000/?filename=path/to/my/file.txt`  
Reading the file should be in a separate child process, as following:  
*From the main process, send the `filename` (after parsing `req.url`) to the child process to start reading the file in chunks as stream, send every chunk back to the main process and to the response, once the reading stream emits "end" then you should send a signal to the main process to end the response and kill the child process. For more help check the stream API details: `https://nodejs.org/api/stream.html`*
