# project_in_c

# UDP Client-Server Sum Calculator


## Project Description

This project demonstrates a **UDP-based client-server communication system in C** where multiple clients send numbers to a server. The server calculates the **sum** of the numbers received and broadcasts the result back to all clients.

It is a simple yet practical example to understand:

* UDP socket programming in C
* Client-server communication
* Handling multiple clients in a single-threaded server

## File Structure

```
UDP-Client-Server/
│
├── server.c        # UDP server code
├── client1.c       # UDP client 1 code
├── client2.c       # UDP client 2 code
├── client3.c       # UDP client 3 code
└── README.md       # Project documentation
```

## Features

* Handles **3 clients simultaneously**
* Dynamically receives numbers from clients
* Calculates **sum** and broadcasts to all clients
* Easy to extend for more clients

## Requirements

* C compiler (e.g., `gcc`)
* Linux / macOS / Windows (with UDP socket support)

## How to Run

### 1. Compile the server and clients:

```bash
gcc server.c -o server
gcc client1.c -o client1
gcc client2.c -o client2
gcc client3.c -o client3
```

### 2. Start the server:

```bash
./server
```

### 3. Start clients in **separate terminals**:

```bash
./client1
./client2
./client3
```

### 4. Enter a number in each client when prompted.

The server will calculate the sum and broadcast it to all clients.

## Example Output

**Server:**

```
Server is running...

Waiting for 3 clients...
Received 5 from 127.0.0.1:54321
Received 10 from 127.0.0.1:54322
Received 7 from 127.0.0.1:54323
Sum = 22
Result broadcasted to all clients.
```

**Client 1:**

```
Client 1: Enter a number: 5
Client 1: Received Sum = 22
```

**Client 2:**

```
Client 2: Enter a number: 10
Client 2: Received Sum = 22
```

**Client 3:**

```
Client 3: Enter a number: 7
Client 3: Received Sum = 22
```

## License

This project is **open-source** and free to use under the MIT License.
