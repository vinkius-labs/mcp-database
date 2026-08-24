# Ahnentafel Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ahnentafel-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Generate deterministic ancestor numbering and relationship paths using the Ahnentafel system.

## Description
This MCP server provides a mathematical engine for genealogical lineage management. It uses the standardized Ahnentafel convention to assign unique, deterministic numbers to ancestors. Users can use `calculate_ahnentafel_numbers` to process a list of relatives, `get_relationship_path` to trace the lineage from a subject to a specific ancestor, and `validate_pedigree_integrity` to ensure the genealogical tree is mathematically sound and free of contradictions.


## Available Tools (3)
- **calculate_ahnentafel_numbers**: Assign a unique, deterministic Ahnentafel number to every person provided in a flat list of ancestral relationships
- **get_relationship_path**: Find the specific genealogical path required to reach a specific ancestor from the subject
- **validate_pedigree_integrity**: Verify that a provided set of ancestors adheres to the strict rules of the Ahnentafel system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ahnentafel Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate Ahnentafel numbers for: John (father), Mary (mother), and Robert (paternal grandfather)."

**🤖 AI Agent:**
> John: 2, Mary: 3, Robert: 4.

---

**👤 You:**
> "What is the relationship path for ancestor number 4?"

**🤖 AI Agent:**
> Father -> Paternal Grandfather.

---

**👤 You:**
> "Check if this pedigree is valid: [{"name": "John", "ahnentafelNumber": 2}]"

**🤖 AI Agent:**
> The pedigree is invalid because the mother (number 3) is missing.


## ❓ FAQ

**Q: What is the Ahnentafel system?**
It is a standardized numbering system where the subject is 1, the father is 2N, and the mother is 2N+1.

**Q: How do I verify my family tree is correct?**
You can use the `validate_pedigree_integrity` tool to check for mathematical contradictions or missing links in your data.

**Q: Can I find the path to a specific ancestor?**
Yes, the `get_relationship_path` tool provides the exact sequence of parental steps to reach any ancestor number.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ahnentafel-generator](https://vinkius.com/ai-agent-connect/ahnentafel-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ahnentafel Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ahnentafel-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ahnentafel Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ahnentafel-generator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
