# Gladly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gladly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate customer support workflows via Gladly — manage agents, search knowledge base answers, and update content directly.

## Description
Connect your **Gladly** platform to any AI agent to streamline your customer service operations and knowledge management through natural language.

### What you can do

- **Agent Management** — List all agents in your organization, retrieve specific profiles, and manage call recording statuses.
- **Knowledge Base Search** — Instantly search through consumer-facing public answers to find relevant help articles.
- **Answer Lifecycle** — Create, update, and delete internal or external answers to keep your support documentation current.
- **Content Localization** — Retrieve and update specific answer content for different languages and formats.
- **Operational Control** — Toggle agent call recording settings to ensure compliance and quality monitoring.

### How it works

1. Subscribe to this server
2. Provide your Gladly Organization ID, Email, and API Token
3. Start managing your support team and knowledge base from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor agent availability and manage recording compliance without leaving the chat interface.
- **Knowledge Base Admins** — quickly update help articles and sync content across multiple languages.
- **CX Operations** — automate the retrieval of public answers to assist in drafting customer responses.


## Available Tools (20)
- **add_answer**: Add a new answer
- **create_business_hours**: Create business hours
- **delete_answer**: Delete an answer
- **delete_business_hours**: Delete business hours
- **get_agent_call_recording**: Get agent call recording status
- **get_agent**: Get a specific Gladly agent
- **get_answer_content**: Get answer content
- **get_business_hours**: Get business hours
- **get_public_answer**: Get a specific public answer
- **list_agents**: List Gladly agents
- **list_audiences**: List audiences
- **list_business_hours**: List business hours
- **list_public_answers**: List public answers
- **search_public_answers**: Search public answers
- **send_email**: Send an email message
- **send_sms**: Send an SMS message
- **update_agent_call_recording**: Update agent call recording status
- **update_answer_content**: Add or update answer content
- **update_answer**: Update an existing answer
- **update_business_hours**: Update business hours


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gladly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active agents in our Gladly organization."

**🤖 AI Agent:**
> I've retrieved the agent list. You currently have 12 agents active, including 'Sarah Miller' (ID: ag_123) and 'James Wilson' (ID: ag_456). Would you like to see details for a specific agent?

---

**👤 You:**
> "Search public answers for 'shipping policy' in org 5521."

**🤖 AI Agent:**
> Searching... I found 3 relevant public answers. The top result is 'Standard Shipping Times' (ID: ans_99). Would you like me to fetch the full content of this answer?

---

**👤 You:**
> "Check the call recording status for agent ag_123."

**🤖 AI Agent:**
> The call recording status for agent ag_123 is currently set to 'Enabled'. Would you like to disable it?


## ❓ FAQ

**Q: Can I enable or disable call recording for a specific agent using this tool?**
Yes! Use the `update_agent_call_recording` tool by providing the Agent ID and setting the recording boolean. This allows you to manage compliance settings directly via the AI.

**Q: How do I search for help articles in our public knowledge base?**
You can use the `search_public_answers` tool. Just provide your Organization ID and the search query, and the agent will return the most relevant public-facing articles.

**Q: Is it possible to update the actual text content of an existing answer?**
Absolutely. Use the `update_answer_content` tool with the Answer ID, language code, and the new content payload to modify documentation across different languages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gladly](https://vinkius.com/mcp/gladly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gladly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gladly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gladly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gladly": {
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
