# llm-agent-poc
This is a proof of concept of an LLM agent using a simple JS and HTML approach.

Key Features
🤖 Core Agent Logic

JavaScript implementation of the Python loop logic you provided
Continuous reasoning loop that processes LLM output and tool calls
OpenAI-style function calling interface

🛠️ Three Tool Integrations

Google Search API - Returns snippet results (mock implementation included)
AI Pipe API - Flexible AI workflow proxy (mock implementation)
JavaScript Code Execution - Sandboxed JS execution with results display

🎨 User Interface

Bootstrap-based clean UI with model picker
Real-time conversation display with different message types
Error handling with bootstrap alerts
Keyboard shortcuts (Enter to send)

⚡ Architecture

Minimal, hackable codebase as requested
Tool calls displayed with visual indicators
Results formatted and color-coded
Conversation persistence during session

How It Works

User Input: Type a message and the agent processes it
LLM Processing: The agent sends conversation + tools to LLM
Tool Execution: If LLM requests tools, they're executed automatically
Loop Continuation: Process continues until no more tools are needed
User Turn: Agent waits for next user input

Example Usage
Try these sample inputs to see the agent in action:

"Search for information about IBM"
"Calculate 2 + 2 * 3 using code"
"Use AI to analyze market trends"

Mock vs Real Implementation
The current version includes mock implementations for the APIs to demonstrate functionality. To make it production-ready, you would:

Replace the mock LLM call with actual OpenAI/Anthropic API calls
Integrate real Google Custom Search API
Connect to actual AI Pipe service
Add proper API key management and security

The architecture is designed to make these transitions straightforward - just replace the mock functions with real API calls while keeping the same interface.
