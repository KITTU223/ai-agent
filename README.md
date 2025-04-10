# AI Agent for Automated Tweeting

This project is an AI-powered agent that can tweet on your behalf. It uses modern APIs and tools to interact with Twitter and generate meaningful tweets using AI.

## Features
- Authenticate with Twitter API.
- Generate AI-based tweets using Gemini AI.
- Post tweets programmatically.
- Interactive chat interface with tool integration.

## Tech Stack
- **Node.js**: Backend runtime environment.
- **Express.js**: Web framework for building the API.
- **Twitter API**: For posting tweets and managing Twitter interactions.
- **Gemini API**: For AI-based content generation.
- **Model Context Protocol (MCP)**: For tool integration and communication.
- **dotenv**: For managing environment variables securely.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/KITTU223/ai-agent
   cd ai-agent
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add the following:
   ```
   TWITTER_API_KEY=<your-twitter-api-key>
   TWITTER_API_SECRET=<your-twitter-api-secret>
   TWITTER_ACCESS_TOKEN=<your-twitter-access-token>
   TWITTER_ACCESS_SECRET=<your-twitter-access-secret>
   GEMINI_API_KEY=<your-gemini-api-key>
   ```

4. Run the server:
   ```bash
   npm run server
   ```

5. Run the client:
   ```bash
   npm run client
   ```

## Project Structure

- **server/index.js**: Sets up the MCP server and defines tools for interacting with Twitter.
- **server/mcp.tool.js**: Contains the logic for posting tweets using the Twitter API.
- **client/index.js**: Implements the client-side logic for interacting with the MCP server and Gemini AI.

## Usage

### Server
The server provides tools for:
- Adding two numbers (`addTwoNumbers`).
- Posting tweets (`createPost`).

### Client
The client connects to the server and uses Gemini AI to generate responses. It can call tools defined on the server, such as posting tweets.

### Example Workflow
1. Start the server.
2. Run the client.
3. Interact with the AI agent via the terminal. The agent can generate tweets and post them on your behalf.

## License
This project is licensed under the MIT License.