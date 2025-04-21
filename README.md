<h1 align="center">🧠 Custom MCP Server Demo</h1>

This project is a Custom MCP (Model Context Protocol) Server built using Python, It’s designed to demonstrate how to create a custom server that communicates using the Model Context Protocol (MCP) — a simple, custom-designed protocol useful for building flexible communication systems between clients and servers.


## 📌 What is this project about?
This project helps you understand how to:

 - Build a custom server using Python's socket library

 - Implement a custom protocol (MCP) to handle communication between clients and the server

 - Manage client connections and message handling in a structured way

 - Send and receive custom commands and data with context-aware processing

It is a learning base for creating more complex client-server systems, such as multiplayer games, chat applications, or custom networked tools.

## 🚀 Features

 - 🌐 TCP-based custom server built in Python

 - 🔄 Model Context Protocol: structured message handling

 - 📡 Real-time communication between client and server

 - 🧩 Easy to extend with new message types or functionalities

 - 🧪 Great for learning networking, protocol design, and server architecture


## 🔧 Requirements

 - Python 3.8+

 - Basic understanding of networking (sockets, TCP)

 - No external dependencies required


## 🛠 How to Run

1. Clone the repository:

       git clone https://github.com/Eltaf-azizi/Custom-MCP-Server-Demo.git
       cd custom-mcp-server
   
3. Run the server:

       python server.py


## 💡 How the Protocol Works (MCP)

The Model Context Protocol is a custom-defined protocol where each message includes:

1. A model: What kind of data is being sent (e.g., "chat", "move", "state")

2. A context: Additional metadata to help interpret the model

3. The data: The actual payload/message

Example message structure (as JSON over TCP):

    {
         "model": "chat",
         "context": "user",
         "data": "Hello, world!"
    }
The server parses these messages and responds accordingly, making it easy to handle multiple types of client interactions in a clean and scalable way.
