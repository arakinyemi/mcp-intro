# mcp-intro
This is an introductory project to the Model Context Protocol (MCP)

I created an MCP server that retrieves information about weather alerts and forecasts from the National Weather Service and provides it as context to a custom-built Claude MCP Client

To run it, follow these steps
Step 1: Clone this repository
```bash
git clone "https://github.com/arakinyemi/mcp-intro"
```
Step 2: Setup the server
```bash
cd mcp-intro
cd weather
```

Save the 
Step 3: Create a virtual environment (Install uv if you haven't already)
```bash
uv venv
source .venv/bin/activate
```
Step 4: Setup the client
```bash
cd /mcp-intro/mcp-client
uv venv
source .venv/bin/activate
```
Create a .env file
Go to Anthropic and retrieve your api key
Save it as `ANTHROPIC_API_KEY` 

Step 5: Run the client
```bash
uv run client.py ../weather/weather.py
```
