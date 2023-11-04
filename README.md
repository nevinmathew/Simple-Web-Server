# Simple-Web-Server

This is a simple Golang web server application that serves static files and provides a few basic HTTP endpoints. It demonstrates the use of the Go programming language for building web applications.

## Table of Contents

- [Features](#features)
- [Usage](#usage)

## Features

- **Static File Server**: The web server serves static files from the `./static` directory, which can be useful for hosting HTML, CSS, JavaScript, and other assets for a website.

- **"Hi" Endpoint**: Accessing the `/hi` endpoint responds with a simple "Hi" message, showcasing how to handle HTTP requests and provide responses.

- **Increment Counter Endpoint**: Accessing the `/increment` endpoint increments a counter and returns the updated counter value. This demonstrates the use of mutexes to safely manipulate shared variables in a multi-threaded environment. The use of a mutex highlights the importance of guarding against race conditions in web server applications.

## Usage

- Access the static files by visiting the root URL (e.g., [http://localhost:5000/](http://localhost:5000/)).

- Get a "Hi" message by visiting [http://localhost:5000/hi](http://localhost:5000/hi).

- Increment the counter by visiting [http://localhost:5000/increment](http://localhost:5000/increment). Each time you access this endpoint, the counter value will increase and be displayed on the page, with proper locking to avoid race conditions.

