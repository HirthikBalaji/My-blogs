# Getting Started

Follow these steps to set up and run the Smart Executive Mail application.

## System Requirements

- **Node.js**: Version 18 or higher.
- **Ollama**: Required for AI-powered curation and RAG features.
  - Download from [ollama.com](https://ollama.com).
  - Ensure you have the `llama3.2` model pulled:
  - 
    
```bash
    ollama run llama3.2
```

## Installation

1. Clone the repository to your local machine.
2. No external NPM dependencies are required for the core MCP server as it uses native ES modules.
3. If you intend to use the web dashboard, you may need to run:
   ```bash
   npm install
   ```

## Running the Application

### Web Dashboard
To start the professional executive dashboard:
```bash
npm start
```
This will launch the [[User-Interface|Executive Dashboard]] and the API server.

### MCP Server (Standalone)
To start the server in MCP mode for integration with Claude:
```bash
npm run start:mcp
```

## Data Preparation

Before the system can provide insights, you need to provide your email data in a specific JSON format. See the [[Data-Ingestion]] guide for details on the schema and how to load your data.

---
*Back to [[Introduction]]. See also: [[MCP-Integration]].*
