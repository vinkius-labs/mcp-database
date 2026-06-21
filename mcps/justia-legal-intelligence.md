# Justia Legal Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/justia-legal-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Universal legal intelligence — search cases, statutes, and lawyers via AI.

## Description
Equip your AI agent with the definitive source for US legal data through the **Justia** MCP server. This integration provides access to a massive database of legal cases, statutes, and professional records. Your agent can search for specific court cases by topic, retrieve state-level statutes, and find information about legal professionals. Whether you are conducting legal research, auditing compliance requirements, or exploring judicial history, your agent acts as a dedicated legal researcher through natural conversation.

### What you can do

- **Case Search** — Find US legal cases by keyword, topic, or jurisdiction.
- **Statute Retrieval** — Access state-specific laws and statutes for all 50 US states.
- **Lawyer Discovery** — Search the professional database for qualified legal practitioners.
- **Legal Auditing** — Summarize complex legal findings and historical precedents.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying legal data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Lawyers & Legal Professionals** — quickly verify case details and state laws.
- **Law Students** — research judicial history and statutory requirements for assignments.
- **Business Owners** — check compliance and state-specific legal frameworks.
- **Journalists** — pull reliable legal data for investigative reporting.


## Available Tools
- **get_state_statutes**: Get statutes for a specific US state
- **search_legal_cases**: Search for legal cases on Justia


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Justia Legal Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for legal cases related to 'free speech' in California."

**🤖 AI Agent:**
> Searching the Justia database... I've found several landmark cases related to free speech in the California jurisdiction. Would you like to see the case titles or their specific summaries?

---

**👤 You:**
> "What are the current statutes for 'tenant rights' in New York?"

**🤖 AI Agent:**
> Retrieving statutes for New York... I've found several sections under the NY Real Property Law related to tenant rights, including security deposits and eviction procedures. Would you like a summary of a specific section?

---

**👤 You:**
> "Find lawyers specialized in 'environmental law' in Seattle."

**🤖 AI Agent:**
> Searching the professional database... I've found a list of qualified environmental law practitioners in Seattle. I can provide their names and practice details.


## ❓ FAQ

**Q: Can I find medical malpractice cases?**
Yes! Use the `search_legal_cases` tool with the query 'medical malpractice'. The response will include a list of relevant cases and summaries.

**Q: Are the statutes available for all 50 states?**
Yes. Justia provides comprehensive access to the statutes and codes for all 50 US states. Use the `get_state_statutes` tool with the specific state name.

**Q: Does this include recent Supreme Court decisions?**
Yes. The Justia database is updated with recent judicial opinions and decisions from federal and state courts, including the US Supreme Court.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/justia-legal-intelligence](https://vinkius.com/mcp/justia-legal-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Justia Legal Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `justia-legal-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Justia Legal Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "justia-legal-intelligence": {
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
