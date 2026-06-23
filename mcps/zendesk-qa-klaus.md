# Zendesk QA (Klaus) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zendesk-qa-klaus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Export QA reviews, search conversations, and import ticket data via the Klaus (Zendesk QA) API.

## Description
Connect your **Zendesk QA** (formerly Klaus) account to any AI agent to automate your customer service quality assurance workflows. This MCP server enables your agent to export quality scores, search for reviewed conversations, and import external ticket data directly from natural language interfaces.

### What you can do

- **Review Extraction** — List all quality assurance reviews and internal quality scores (IQS) account-wide or by workspace
- **Workspace Management** — List all available workspaces to organize your QA processes and review assignments
- **Conversation Discovery** — Search for specific customer interactions to identify which ones have been graded
- **Data Integration** — Import conversation data and agent profiles from external platforms for grading in Zendesk QA
- **Record Maintenance** — Permanently remove ticket data from the QA platform via simple commands

### How it works

1. Subscribe to this server
2. Enter your Zendesk Subdomain and QA API Token
3. Start managing your support quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — Monitor support quality trends and export review data for reporting via natural language
- **Support Leads** — Quickly search for agent reviews and identify areas for improvement from your dev tools
- **Operations Teams** — Automate the synchronization of external ticket data into the QA platform effortlessly


## Available Tools (7)
- **delete_qa_tickets**: Remove specific ticket data from the QA platform
- **import_qa_tickets**: Import conversation data into Zendesk QA for review
- **import_qa_users**: Sync agents and managers into Zendesk QA
- **list_all_reviews**: List all quality assurance reviews account-wide
- **search_qa_conversations**: Search for conversations in Zendesk QA
- **list_workspace_reviews**: List reviews for a specific workspace
- **list_qa_workspaces**: Use this to identify workspace IDs for exporting reviews.

List all Zendesk QA workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zendesk QA (Klaus)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zendesk QA workspaces."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have 3 active environments: 'English Support', 'Spanish Support', and 'Technical Escalations'. Which one would you like to access?

---

**👤 You:**
> "Show recent QA reviews for the 'English Support' workspace (ID: '123')."

**🤖 AI Agent:**
> I found 10 recent reviews for the English Support workspace. The average Internal Quality Score (IQS) is 92%. Notable recent reviews include tickets #ORD-987 and #TECH-101.

---

**👤 You:**
> "Search for reviewed conversations associated with client email 'user@example.com'."

**🤖 AI Agent:**
> I've searched your account and found 2 conversations for 'user@example.com' that have been graded. Ticket #12345 received a score of 100% and Ticket #12346 received a score of 85%.


## ❓ FAQ

**Q: How do I find my Workspace ID?**
Use the `list_qa_workspaces` tool to retrieve a comprehensive list of all workspaces in your account along with their unique IDs.

**Q: Can I export reviews for a specific date range?**
Yes, you can provide a `params` string (e.g., `fromDate=2023-01-01&toDate=2023-01-31`) to the list reviews tools to filter by date.

**Q: What is the difference between the Export and Import APIs?**
The Export API is for retrieving QA results (scores and reviews), while the Import API is for pushing conversation data and user profiles into the platform for review.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zendesk-qa-klaus](https://vinkius.com/mcp/zendesk-qa-klaus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zendesk QA (Klaus)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zendesk-qa-klaus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zendesk QA (Klaus)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zendesk-qa-klaus": {
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
