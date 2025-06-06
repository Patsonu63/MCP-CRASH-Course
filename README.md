# MCP-CRASH-Course
This is a basic example of a Model Context Protocol (MCP) server implementation that demonstrates core functionality including tools and resources.
setup
Initialize the project (Go to any local folder and launch powershell or cmd):

uv init mcp-server-basic
cd mcp-server-basic

Create virtual environment and activate it
  uv venv
  .venv\Scripts\activate
  
  Install dependencies:
uv add "mcp[cli]"
or uv add -r requirements.txt

Features
The server implements the following features:

Tools
add(a: int, b: int): Adds two numbers
subtract(a: int, b: int): Subtracts second number from first
Resources
greeting://{name}: Returns a personalized greeting
Running the Server
To run the server with the MCP Inspector for development:

uv run mcp dev main.py

To run the server normally:

uv run mcp run
To install the server in Claude desktop app:

uv run mcp install main.py
MCP connect in VS code
Open folder/mcp-server-basic in vs code
open terminal and run below command :
uv run main.py
Click Cntrl+Shift+I to launch chat in vs code
Do login with Github and setup
Folow the below steps (two way to add mcp configuration for vs code user settings):
Project Structure
main.py: Main server implementation with tools and resources
pyproject.toml: Project configuration and dependencies
