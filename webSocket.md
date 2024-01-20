# WebSocket Documentation

## Overview

WebSocket is a communication protocol that provides full-duplex communication channels over a single, long-lived connection. Unlike traditional request-response mechanisms like HTTP, WebSocket enables real-time bidirectional communication between clients and servers.

## Table of Contents

- [Getting Started](#getting-started)
  - [Establishing a WebSocket Connection](#establishing-a-websocket-connection)
  - [WebSocket URL](#websocket-url)
- [Communication Protocol](#communication-protocol)
  - [WebSocket Handshake](#websocket-handshake)
  - [Data Frames](#data-frames)
- [Security Considerations](#security-considerations)
  - [Secure WebSocket (WSS)](#secure-websocket-wss)
  - [Authentication](#authentication)
- [Advanced Features](#advanced-features)
  - [Subprotocols](#subprotocols)
  - [Ping/Pong Frames](#pingpong-frames)
- [Client and Server Implementations](#client-and-server-implementations)
  - [JavaScript (Client)](#javascript-client)
  - [Node.js (Server)](#nodejs-server)
- [Troubleshooting](#troubleshooting)
  - [Common Issues](#common-issues)
  - [Handling Errors](#handling-errors)

## Getting Started

### Establishing a WebSocket Connection

To initiate a WebSocket connection, clients send a WebSocket handshake request, and servers respond with an acceptance or rejection. Once established, the connection remains open for further communication.

```javascript
// JavaScript example
const socket = new WebSocket('ws://example.com/socket');
```

### WebSocket URL

The WebSocket URL consists of the WebSocket scheme (`ws` or `wss` for secure), the host, and optional path. For example:
- `ws://example.com/socket`
- `wss://secure.example.com/chat`

## Communication Protocol

### WebSocket Handshake

During the WebSocket handshake, the client sends an HTTP request, and the server responds with an HTTP 101 status code, indicating a successful upgrade to WebSocket.

### Data Frames

WebSocket communication occurs through data frames. Frames can be text, binary, or control frames for various purposes.

```javascript
// Sending a message
socket.send('Hello, WebSocket!');

// Handling incoming messages
socket.onmessage = (event) => {
  const message = event.data;
  console.log('Received:', message);
};
```

## Security Considerations

### Secure WebSocket (WSS)

For secure communication, use the `wss` scheme. This encrypts the data exchanged between the client and server.

### Authentication

Implement proper authentication mechanisms to secure your WebSocket connections. Authenticate users or devices based on your application's requirements.

## Advanced Features

### Subprotocols

WebSocket allows the use of subprotocols to define a specific communication protocol between the client and server.

### Ping/Pong Frames

Ping and pong frames can be used to check the health of the WebSocket connection and detect potential issues.

## Client and Server Implementations

### JavaScript (Client)

For JavaScript clients, use the native `WebSocket` API in web browsers.

```javascript
const socket = new WebSocket('ws://example.com/socket');
```

### Node.js (Server)

In Node.js, use libraries like `ws` for WebSocket server implementation.

```javascript
const WebSocket = require('ws');
const wss = new WebSocket.Server({ port: 8080 });

wss.on('connection', (socket) => {
  console.log('Client connected');
});
```

## Troubleshooting

### Common Issues

- Ensure correct WebSocket URL.
- Check for proper server implementation.
- Verify WebSocket handshake responses.

### Handling Errors

Handle errors gracefully by listening to the WebSocket `onerror` event.

```javascript
socket.onerror = (error) => {
  console.error('WebSocket Error:', error);
};
```

This documentation provides a basic understanding of WebSocket. Refer to the [WebSocket RFC](https://tools.ietf.org/html/rfc6455) for detailed specifications.
```
