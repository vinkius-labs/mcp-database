# Breezy HR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/breezy-hr-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage recruitment workflows via Breezy HR — list companies, track job positions, and manage candidates directly from any AI agent.

## Description
Connect your **Breezy HR** account to any AI agent and streamline your recruitment pipeline through natural conversation.

### What you can do

- **Companies & Positions** — List all organizational companies and fetch active job openings directly from Breezy HR
- **Candidate Tracking** — Query candidates for specific roles and view their application history and status
- **Applicant Management** — Add new candidates to your pipeline instantly with name and contact details
- **Deep Inspection** — Fetch detailed metadata for companies, positions, and individual candidates to understand hiring progress
- **Application History** — List all applications associated with a candidate to track their journey across different roles

### How it works

1. Subscribe to this server
2. Enter your Breezy HR API Key
3. Start managing your hiring process from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & HR Managers** — instantly retrieve candidate statuses and list open positions without switching tabs
- **Hiring Managers** — check candidate details and application history straight from your workflow
- **Talent Acquisition Leads** — automate the retrieval of recruitment data to orchestrate hiring across multiple companies


## Available Tools (8)
- **add_candidate**: Add a new candidate to a position
- **get_candidate**: Get details for a specific candidate
- **get_company**: Get details for a specific company
- **get_position**: Get details for a specific position
- **list_applications**: List applications for a candidate
- **list_candidates**: List candidates for a position
- **list_companies**: List Breezy HR companies
- **list_positions**: List positions for a company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breezy HR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all companies in my Breezy HR account."

**🤖 AI Agent:**
> I've retrieved your companies. You have access to: 'Acme Corp' (ID: 5a1b2c) and 'Global Tech' (ID: 3d4e5f). Which one would you like to explore?

---

**👤 You:**
> "Show me the candidates for the 'Senior Developer' position (ID: pos_123) in company 5a1b2c."

**🤖 AI Agent:**
> Fetching candidates for 'Senior Developer'... I found 3 candidates: Alice Smith, Bob Jones, and Charlie Brown. Would you like the details for any of them?

---

**👤 You:**
> "Add a new candidate named John Doe with email john@example.com to position pos_123 in company 5a1b2c."

**🤖 AI Agent:**
> Successfully added John Doe to the 'Senior Developer' position. The candidate record has been created in Breezy HR.


## ❓ FAQ

**Q: Can I see the full details of a specific candidate using their ID?**
Yes! Use the `get_candidate` tool by providing the Company ID, Position ID, and Candidate ID. The agent will return all available profile information and metadata for that candidate.

**Q: How do I list all open job positions for a specific company?**
Simply use the `list_positions` tool with the target Company ID. It will return a list of all job openings associated with that company account.

**Q: Is it possible to add a new candidate to a position directly through the AI?**
Yes, you can use the `add_candidate` action. You'll need to provide the Company ID, Position ID, and the candidate's name (email is optional but recommended) to create the record.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/breezy-hr-alternative](https://vinkius.com/mcp/breezy-hr-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breezy HR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breezy-hr-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breezy HR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breezy-hr-alternative": {
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
