# Java HTTP Name Server

This project provides a simple Java HTTP server that listens on port 8080 and responds to GET requests at `/name?name=YourName` with a personalized greeting.

## How to Run

1. Make sure you have Java (JDK 8 or later) installed.
2. Open a terminal in this project directory.
3. Compile the server:
   ```sh
   javac NameServer.java
   ```
4. Run the server:
   ```sh
   java NameServer
   ```
5. Open your browser or use curl to test:
   - [http://localhost:8080/name?name=Alice](http://localhost:8080/name?name=Alice)

## Example

```
GET /name?name=Alice
Response: Hello, Alice!
```

## Notes
- Only GET requests are supported.
- If no `name` parameter is provided, the server responds with `Hello, Guest!`.
