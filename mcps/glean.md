# Glean MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glean)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Empower enterprise search via Glean — search across all SaaS apps, retrieve AI answers, manage custom indexing, and handle chat directly from any AI agent.

## Description
Connect your **Glean** enterprise account to any AI agent and take full control of your corporate-wide knowledge discovery and AI-powered workspace through natural conversation.

### What you can do

- **Corporate Discovery Orchestration** — Identify bounded CRM records and extract explicitly attached REST arrays targeting `/search` to find knowledge mapped across all SaaS applications natively
- **Live AI Answer Retrieval** — Enumerate explicitly attached structured rules to fire RAG mechanisms, returning pure AI-generated blocks distilled from your company data limitlessly
- **Multi-Source Filtering** — Perform structural extraction of properties by hardcoding explicit filters parsing only specific datasources like Jira, Confluence, or Slack nodes synchronousy
- **People & Identity Discovery** — Retrieve corporate active directory information, matching user skills, roles, and names directly to generate hard customer bindings natively
- **Intelligent Chat Orchestration** — Commands explicit REST targets checking `/chat` to manage ongoing text streams while maintaining historical thread mapping for complex reasoning
- **Knowledge Ingestion & Indexing** — Upload massive custom text properties directly routing into corporate search logic to verify internal documentation boundaries securely
- **Predictive Autocomplete** — Discovers disconnected physical limits executing `/autocomplete` to predict precise page destinations from partial prefixes flawlessly
- **Data Deletion Oversight** — Explains explicitly mapped arrays checking `/delete` to remove indexed documents permanently and block future retrieval vectors

### How it works

1. Subscribe to this server
2. Enter your Glean Domain (e.g., 'yourcompany') and API Token (found in your Glean Admin Settings)
3. Start searching your company's knowledge from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers & Researchers** — quickly find documentation and answers across all company apps without manual searching
- **HR & Ops Teams** — search for people by skills or roles and monitor trending company content using natural language
- **Developers** — index custom documentation and test AI chat workflows directly from the IDE or chat interface
- **Leadership Teams** — audit organizational knowledge and verify AI-generated answers in real-time


## Available Tools (10)
- **custom_request**: ` merging physical POST arrays strictly.

Identify precise active arrays spanning native Hold parsing
- **delete_document**: Inspect deep internal arrays mitigating specific Plan Math
- **search_datasource**: g.

Perform structural extraction of properties driving active Account logic
- **index_document**: Identify precise active arrays spanning native Gateway auth
- **search_people**: Provision a highly-available JSON Payload generating hard Customer bindings
- **search_docs**: Identify bounded CRM records inside the Headless Glean Platform
- **get_suggestions**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **get_answer**: Enumerate explicitly attached structured rules exporting active Billing
- **autocomplete**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **chat_completion**: Dispatch an automated validation check routing explicit Gateway history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glean** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Q2 hiring plan' in all apps"

**🤖 AI Agent:**
> Searching corporate knowledge... I found 3 documents across Google Drive and Confluence. The most relevant is 'Final Hiring Plan Q2' (ID: doc_abc). Would you like me to get an AI-generated summary of its contents?

---

**👤 You:**
> "Who knows about 'React Native' in my company?"

**🤖 AI Agent:**
> Searching people... I found 2 colleagues with 'React Native' listed in their skills: Alice Smith (Mobile Lead) and Bob Johnson (Senior Engineer). Would you like their contact details or recent Slack activity?

---

**👤 You:**
> "Get AI answer for: 'What is our expense policy for business travel?'"

**🤖 AI Agent:**
> Synthesizing answer... According to the Employee Handbook in Confluence, our business travel policy allows for $50/day in meal reimbursements and requires all flights to be booked via the Corporate Portal at least 2 weeks in advance.


## ❓ FAQ

**Q: Can my agent get direct AI answers based on my company's data via Glean?**
Yes. Use the 'get_answer' tool. It fires Glean's internal RAG mechanisms to retrieve a pure AI-generated response distilled from your indexed company knowledge flawlessly.

**Q: How do I search for experts in my company by their skills via chat?**
Use the 'search_people' tool. The agent will retrieve information from your corporate active directory, matching user profiles, skills, and names to help you find the right colleague natively.

**Q: Can I index my own custom documents in Glean through the agent?**
Absolutely. Use the 'index_document' tool. Provide a JSON object defining the ID, Title, and text content. The agent will route the payload into Glean's search logic synchronously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glean](https://vinkius.com/mcp/glean)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glean** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `glean` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glean** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glean": {
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
