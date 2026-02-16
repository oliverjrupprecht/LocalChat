```
 /$$                                     /$$  /$$$$$$  /$$                   /$$    
| $$                                    | $$ /$$__  $$| $$                  | $$    
| $$        /$$$$$$   /$$$$$$$  /$$$$$$ | $$| $$  \__/| $$$$$$$   /$$$$$$  /$$$$$$  
| $$       /$$__  $$ /$$_____/ |____  $$| $$| $$      | $$__  $$ |____  $$|_  $$_/  
| $$      | $$  \ $$| $$        /$$$$$$$| $$| $$      | $$  \ $$  /$$$$$$$  | $$    
| $$      | $$  | $$| $$       /$$__  $$| $$| $$    $$| $$  | $$ /$$__  $$  | $$ /$$
| $$$$$$$$|  $$$$$$/|  $$$$$$$|  $$$$$$$| $$|  $$$$$$/| $$  | $$|  $$$$$$$  |  $$$$/
|________/ \______/  \_______/ \_______/|__/ \______/ |__/  |__/ \_______/   \___/  
```

A minimalist Terminal User Interface (TUI) for interacting with local LLMs. A Python application utilizing Textual for the UI, with Ollama and SQLite3 handling the backend. This app provides a clean chat experience directly in your terminal.

**Key Features:**
- Local-First: Your data never leaves your machine. It talks directly to your local Ollama instance.
- Real-time Markdown Rendering: Model responses are and formatted instantly from Markdown. (Most modern models reply in Markdown format) 
- Persistent Session Logging: Chat sessions are logged in an internal Sqlite database. Sessions can be rebooted if necessary.
- Streaming Responses: No waiting for the full block; get tokens as they are generated for a fluid conversation. (not fully implemented)
- Automatic Model Management: Loads model on startup and frees it from memory when leaving the application.

**Implementation Details:**
- The multithreaded implementation of model calls and large IO operations means that the UI remains snappy.

**Requirements:**
- Users must have Ollama and Homebrew installed. Ollama should be running as a daemon. Personally, I use Homebrew's services functionality.

**Installation:**
- This project is currently in development.

**Example Use:**

<img width="1431" height="885" alt="Screenshot 2026-02-16 at 12 22 02 pm" src="https://github.com/user-attachments/assets/246137a1-6ea9-4a59-b46f-2d346df993c3" />



