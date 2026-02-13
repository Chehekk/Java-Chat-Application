# Java Multi-User Chat System 💬

A real-time communication platform built from scratch using Java. This project demonstrates the power of **Socket Programming**, **Multithreading**, and **GUI Development** in a Client-Server architecture.

## 🌟 Features
- **Multi-User Support**: Multiple clients can connect to the server simultaneously using threads.
- **Real-Time Broadcasting**: Every message sent is instantly broadcast to all active participants.
- **User-Friendly GUI**: Built with Java Swing, featuring message timestamps and auto-scrolling chat history.
- **System Notifications**: Dynamic alerts when a user joins or leaves the chat.
- **Lightweight & Fast**: Uses raw TCP sockets for low-overhead text communication.

## 🛠️ Tech Stack
- **Language**: Java 21 (or higher)
- **Networking**: Java Sockets (TCP/IP)
- **Concurrency**: Java Threads (Multithreading)
- **GUI Framework**: Java Swing & AWT

## 🏗️ Architecture
The system follows a **Star Topology** with a central Server:
1. **ChatServer**: Listens for incoming socket connections and manages a list of active `ClientHandlers`.
2. **ClientHandler**: A dedicated thread for each connected user to handle incoming data without blocking the server.
3. **ChatClient**: The graphical interface that allows users to connect, type messages, and receive updates.

## 🚀 How to Run

### Prerequisites
- Java Development Kit (JDK) installed.
- Terminal/Command Prompt access.

### Manual Launch
1. **Compile the files:**
   ```bash
   javac ChatServer.java ChatClient.java
   ```
2. **Start the Server:**
   ```bash
   java ChatServer
   ```
3. **Start the Clients (Run this as many times as you want!):**
   ```bash
   java ChatClient
   ```

