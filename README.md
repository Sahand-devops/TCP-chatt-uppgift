# TCP Chat Application

A simple Python TCP chat example consisting of a server and a client. The project demonstrates basic socket programming using TCP over localhost.

## Project Structure

- `server_tcp/`
  - Python server that listens for a single client connection.
  - Receives incoming messages from the client and sends responses.

- `client_tcp/`
  - Python client that connects to the server.
  - Sends messages to the server and displays replies.

## How it Works

1. Start the server first.
2. Start the client and connect to the server at `127.0.0.1:12345`.
3. Type messages in the client prompt to send them to the server.
4. Type messages in the server prompt to reply.
5. Send `hejdå` from either side to close the chat.

## Requirements

- Python 3.x

## Run Instructions

Open two terminal windows.

### Start the server

```bash
cd server_tcp
python server_tcp.py
```

### Start the client

```bash
cd client_tcp
python client_tcp.py
```

## Notes

- Use the same IP and port for both server and client.
- The server accepts one connection at a time.
- The chat session ends when either side sends `hejdå`.

## Improvements

Possible enhancements:

- Add support for multiple clients.
- Use threading for concurrent connections.
- Add message history or user names.
- Add input validation and error handling.
