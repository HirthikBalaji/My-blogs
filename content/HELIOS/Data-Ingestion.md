# Data Ingestion

To populate the [[Core-Features#F3: Knowledge Graph|Knowledge Graph]], you must provide your email data in a JSON format.

## Email JSON Schema

Each email object should follow this structure:

```json
{
  "subject": "URGENT: Budget Approval Required",
  "from": "hod.cs@college.edu",
  "to": "principal@college.edu",
  "cc": "dean@college.edu",
  "date": "2026-03-20T13:59:45+00:00",
  "body": "Plain text or HTML body",
  "message_id": "<unique-id@domain>"
}
```

### Automatic Processing
When you load data, the system automatically:
- Strips HTML from the body.
- Classifies priority (High, Medium, Normal, Low).
- Detects topics (e.g., Accreditation, Placement, Budget).
- Infers departments based on sender/recipient patterns.
- Builds the relationship graph.

## How to Load Data

### Via MCP Tool
If using the [[MCP-Integration|Claude Integration]], use the `load_emails` tool:
```json
{
  "emails": [ /* your array of email objects */ ],
  "reset": false
}
```

### Via Python Script
You can use the provided `load.py` script (if available) to batch-upload data from a local JSON file or `.mbox` export.

---
*Ready to use the system with Claude? Check out [[MCP-Integration]].*
