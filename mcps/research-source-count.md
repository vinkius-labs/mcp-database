# research-source-count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/research-source-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify and categorize research sources by type.

## Description
This MCP server provides tools to analyze collections of research materials. It allows you to perform schema validation, filter sources by specific categories, and generate detailed summaries of source distributions. Use `get_total_source_summary` to see a high-level overview of your entire collection or `get_source_counts` to see the specific distribution of types like Academic, Media, or Technical.


## Available Tools (4)
- **filter_sources_by_type**: Filter sources by a specific type
- **get_source_counts**: Counts supplied sources by source type
- **get_total_source_summary**: Get a summary of total unique sources and their type distribution
- **validate_source_schema**: Validate the schema of the provided sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **research-source-count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many sources do I have for each category in this list: [{"id": "1", "type": "Academic", "title": "Study A"}, {"id": "2", "type": "Media", "title": "News B"}]?"

**🤖 AI Agent:**
> You have 1 Academic source and 1 Media source.

---

**👤 You:**
> "Give me a summary of these sources: [{"id": "1", "type": "Technical", "title": "Doc 1"}, {"id": "2", "type": "Technical", "title": "Doc 2"}]"

**🤖 AI Agent:**
> You have a total of 2 unique sources, with 2 belonging to the Technical category.

---

**👤 You:**
> "Filter the sources to only show me the 'Legal' ones from this list: [{"id": "1", "type": "Legal", "title": "Patent X"}, {"id": "2", "type": "Academic", "title": "Paper Y"}]"

**🤖 AI Agent:**
> {"id": "1", "type": "Legal", "title": "Patent X"}


## ❓ FAQ

**Q: How can I check if my source list is valid?**
You can use the `validate_source_schema` tool to verify that your list of sources contains the required unique identifiers and type classifications.

**Q: Can I see a breakdown of my research types?**
Yes, the `get_source_counts` tool provides a specific count for every category present in your dataset.

**Q: How do I get a total count of all my sources?**
Use the `get_total_source_summary` tool to receive both the total number of unique sources and a breakdown by type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/research-source-count](https://vinkius.com/en/ai-agent-connect/research-source-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **research-source-count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `research-source-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **research-source-count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "research-source-count": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
