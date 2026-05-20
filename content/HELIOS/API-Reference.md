# API Reference

This document provides a summary of the available tools and endpoints within the Smart Executive Mail system.

## MCP Tools

These tools are available when using the system via [[MCP-Integration]].

| Tool | Description | Key Parameters |
|------|-------------|----------------|
| `load_emails` | Ingest email JSON data. | `emails`, `reset` |
| `executive_query` | Natural-language command center. | `query` |
| `get_predictions` | Proactive risk & action predictions. | `urgency_filter` |
| `get_digital_twin` | Institutional health model. | `section` |
| `get_knowledge_graph`| People, threads, and projects. | `view`, `limit` |
| `get_daily_briefing` | Critical morning summary. | - |
| `search_emails` | Full-text search across data. | `query`, `priority_filter` |
| `get_department_health`| Detailed metrics for a specific dept. | `department` |
| `get_escalations` | Active risk and hidden issues. | - |

## REST API Endpoints

When running the [[User-Interface|Web Dashboard]], the following endpoints are available:

- `GET /api/briefing`: Returns the daily executive briefing.
- `GET /api/twin`: Returns the full digital twin status.
- `GET /api/graph`: Returns the knowledge graph summary.
- `POST /api/query`: Processes a natural-language query via RAG.
- `POST /api/curate`: Triggers the AI Strategic Curation.

Detailed Swagger documentation is available at `/docs` when the server is running.

---
*Back to [[Introduction]].*
