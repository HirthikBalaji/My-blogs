# User Interface

The application features a professional, light-themed dashboard designed for high-level executive use.

## Dashboard Overview
The main screen provides an at-a-glance view of the institution's state:
- **Daily Briefing**: Summarizes critical actions and pending approvals.
- **Institutional Health**: Visualizes department workload and stress scores.
- **Predictive Alerts**: Highlights upcoming risks identified by the [[Core-Features#F1: Proactive Executive Intelligence|Behavior Engine]].

## AI Curation Tab
This feature uses the local LLM to provide a strategic overview:
- **Critical Actions**: Extracts immediate priorities.
- **Institutional Risks**: Highlights silent escalations.
- **Key Opportunities**: Surfaces growth areas and collaborations.
- **Refresh Analysis**: Use this button to update the brief with the latest email data.

## Command Center
The natural-language search bar allows for direct querying of the [[Core-Features#F3: Knowledge Graph|Knowledge Graph]]. Answers are generated using RAG, ensuring they are grounded in your specific institutional context.

## API & Documentation
For technical users, the system includes:
- **Swagger UI**: Accessible at `/docs`, providing detailed documentation for all analytical endpoints.
- **JSON Export**: Tools for exporting insights for further analysis.

---
*Next: Learn how to [[Data-Ingestion|load your data]] into the system.*
