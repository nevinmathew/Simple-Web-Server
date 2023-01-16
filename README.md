# Simple-Web-Server

This is a simple web server project created using Golang. This web server application is built using the net/http package.

The parent URL serves a simple static file.

 Due to the fact that web servers are asynchronous, we’ll have to guard our counter using a mutex in order to prevent us from being hit with race-condition bugs. Here it is just being used to highlight that these servers aren’t guarded against race conditions. Navigate to http://localhost:5000/increment and you should see the current count which will be locked, incremented and then unlocked every time you make a request to that page.
