Chat Application - Client Side
This is a simple chat client application developed in C# using Windows Forms. It connects to a server and allows users to send and receive messages.

Features
Connects to a remote server via TCP/IP
Sends messages to the server
Receives messages from the server and displays them in a chat window
Provides real-time message updates
How to Use
Clone or download this repository.
Open the solution in Visual Studio.
Build and run the application.
Dependencies
.NET Framework
Usage
Enter your message in the text box at the bottom of the window.
Click the "Send" button to send the message to the server.
Received messages will appear in the chat window.
Code Overview
The client application consists of the following components:

Form1.cs: The main form of the application, responsible for UI interaction and message handling.
Server_MessageReceived: Method for handling incoming messages from the server.
button1_Click: Event handler for sending messages to the server.
listBox1_SelectedIndexChanged: Method for displaying the current date and time in the console.
Running the Application
To run the application:

Open the solution in Visual Studio.
Build the solution.
Start the application.
Server Configuration
Make sure the server is running and listening on the correct IP address and port (127.0.0.1:54000 by default). Modify the server IP address and port in the Connect method of the OnShown event handler in Form1.cs if necessary.

Support
For any issues or questions, please open an issue in this repository.

Chat Application - Server Side
This is the server component of a simple chat application developed in C++. It listens for incoming connections from clients and relays messages between them.

Features
Listens for incoming connections from clients
Relays messages between clients
Supports multiple simultaneous client connections
How to Use
Clone or download this repository.
Open the solution in Visual Studio.
Build and run the application.
Dependencies
.NET Framework
Usage
Ensure that the server is running and listening for incoming connections.
Client applications can connect to the server using the IP address and port specified in the server configuration.
Code Overview
The server application consists of the following components:

Form1.cs: The main form of the application, responsible for listening for incoming connections and relaying messages between clients.
Server_MessageReceived: Method for handling incoming messages from clients and relaying them to other clients.
OnShown: Event handler for starting the server and listening for incoming connections.
button1_Click: Event handler for sending messages to connected clients.
Running the Application
To run the server application:

Open the solution in Visual Studio.
Build the solution.
Start the application.
Client Configuration
Make sure the client applications are configured to connect to the correct IP address and port (127.0.0.1:54000 by default). Modify the server IP address and port in the client applications if necessary.
