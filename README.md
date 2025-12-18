# TCP File Service – Client/Server Application

## Overview
This project is a Java-based TCP client–server application that implements a simple file service over a reliable byte-stream connection. The system allows a client to remotely interact with files stored on a server through a custom-designed file transfer protocol.

This project was completed for **CS316 – Project 3: Design & Implementation of a TCP File Service** and demonstrates core networking concepts using TCP sockets.

---

## Learning Objectives
- Implement a client–server architecture using TCP
- Design and implement a file transfer protocol
- Apply the TCP byte-stream model for reliable communication
- Handle user input, command parsing, and error conditions

---

## Features
The client supports **five file service commands**, all processed by the server:

- **List** – Display all files available on the server  
- **Delete** – Remove a specified file from the server  
- **Rename** – Rename an existing file on the server  
- **Download** – Download a file from the server to the client  
- **Upload** – Upload a file from the client to the server  

For the **delete**, **rename**, and **upload** commands, the server returns a status code indicating success or failure. Status codes are not required for the **list** or **download** commands.

---

## How It Works
1. The server starts and listens for incoming TCP connections.
2. The client connects using the server’s IP address and port number.
3. The user enters a command in the client program.
4. The client sends a formatted request message to the server.
5. The server processes the request and performs the file operation.
6. The server sends a response or status code back to the client.
7. The client displays the result and closes the connection.
