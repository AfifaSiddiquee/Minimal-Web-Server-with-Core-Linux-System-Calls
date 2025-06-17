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


 ✅ Achievements
Implemented system-level networking operations

Achieved concurrency using multi-processing

Practiced OS-level concepts like process isolation and resource management

⚠️ Limitations
Not scalable for production use (each client handled via fork())

Only supports basic GET requests

No HTTPS or advanced protocol features

No robust error handling or logging

🔮 Future Improvements
Use threads or asynchronous I/O (e.g., select() or epoll) for better scalability

Add support for more HTTP methods (POST, PUT)

Implement HTTPS using SSL/TLS

Integrate logging and error tracking

📚 Learning Outcome
Through this project, I gained hands-on experience in working directly with Linux system calls, deepening my understanding of how operating systems manage processes, network sockets, and resource allocation behind the scenes in real-world applications.
