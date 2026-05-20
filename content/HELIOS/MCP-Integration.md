# MCP Integration

The Smart Executive Mail server supports the **Model Context Protocol (MCP)**, allowing it to integrate seamlessly with AI assistants like Claude Desktop and Claude Code.

## Claude Desktop Configuration

Add the following to your `claude_desktop_config.json`:

**Path (macOS):** `~/Library/Application Support/Claude/claude_desktop_config.json`  
**Path (Windows):** `%APPDATA%\Claude\claude_desktop_config.json`

```json
{
  "mcpServers": {
    "smart-mail-mcp": {
      "command": "node",
      "args": ["/absolute/path/to/smart-mail-mcp/src/index.js"]
    }
  }
}
```

*Note: Replace `/absolute/path/to/` with the actual path on your machine.*

## Claude Code Configuration

To add the server to your Claude Code project:
```bash
claude mcp add smart-mail-mcp node /absolute/path/to/smart-mail-mcp/src/index.js
```

## Available Tools in Claude

Once connected, Claude will have access to several specialized tools:
- **`load_emails`**: Ingest email data.
- **`executive_query`**: Run natural-language queries.
- **`get_daily_briefing`**: Get a summary of the day's priorities.
- **`get_predictions`**: View proactive risk assessments.
- **`get_digital_twin`**: Explore institutional health metrics.

See the [[API-Reference]] for a complete list of tools and their functions.

---
*Back to [[Introduction]].*
