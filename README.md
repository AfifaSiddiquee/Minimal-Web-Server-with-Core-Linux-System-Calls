# 🌐 Minimal Web Server with Core Linux System Calls

**Course:** Operating Systems (CT-353)  
**Department:** Computer Science & Information Technology, NED University  
**Student:** Afifa Siddique  
**Project Type:** Complex Computing Problem (CCP)

## 🔗 Project Overview

This project showcases the development of a basic web server using core **Linux system calls**. It simulates the low-level behavior of HTTP servers by handling TCP connections, spawning child processes for concurrent client handling, and managing request/response operations—all implemented in C using system-level functions.

---

## 🚀 Features

- Processes basic HTTP GET requests  
- Handles multiple clients using `fork()` (multi-processing)  
- Sends a basic HTML response to connected clients  
- Demonstrates usage of raw TCP sockets and system resources  

---

## 🛠️ Technologies Used

- **C Programming Language**  
- **Linux OS**  
- Core System Calls:  
  - `socket()`, `bind()`, `listen()`, `accept()`  
  - `fork()`, `wait()`  
  - `read()`, `write()`, `send()`, `close()`  

---

## 📟 System Calls in Action

### 🔌 Networking
- `socket()` – Create socket for communication  
- `bind()` – Assign socket to IP and port  
- `listen()` – Listen for incoming client connections  
- `accept()` – Accept client connection requests  

### 👥 Process Management
- `fork()` – Spawn child process per client  
- `wait()` – Handle cleanup of zombie processes  

### 📁 File Management
- `read()` – Read HTTP request from client  
- `write()` / `send()` – Send HTTP response to client  

---

## 📥 Sample Response

The server responds with a simple HTML page:

```http
HTTP/1.1 200 OK
Content-Type: text/html

<html><body><h1>Hello, World!</h1></body></html>

