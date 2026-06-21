# SketricGen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sketricgen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI agents to SketricGen to run multi-agent workflows, manage knowledge bases, debug traces, and interact with contacts.

## Description
Empower your AI agents to securely orchestrate complex workflows using the SketricGen platform. With 18 dedicated tools, your AI can now programmatically trigger multi-agent tasks, inject relevant contacts into context, construct searchable knowledge bases, and granularly inspect execution traces.

### What you can do
- Execute complex multi-agent workflows programmatically
- Create and query vector-searchable knowledge bases
- Debug executions with full tracing capabilities
- Track tool calls and credit consumption per run
- Access and manage CRM-style contact profiles
- Maintain distinct conversation histories

### How it works
1. Subscribe to this server
2. Enter your SketricGen API Key (found in your account dashboard)
3. Start deploying orchestrated multi-agent systems via Vinkius

### Who is it for?
Designed for AI engineers, prompt designers, and automation teams seeking an advanced orchestration layer with full traceability for complex agentic workflows.


## Available Tools (18)
- **check_sketricgen_status**: Verify connectivity
- **delete_conversation**: Delete conversation
- **get_agent**: Get agent details
- **get_contact**: Get contact details
- **get_conversation**: Get conversation
- **get_knowledge_base**: Get knowledge base
- **get_trace_credits**: Get trace credit usage
- **get_trace**: Get trace details
- **get_workflow**: Get workflow details
- **list_agents**: List AI agents
- **list_contacts**: List contacts
- **list_conversations**: List conversations
- **list_knowledge_bases**: List knowledge bases
- **list_templates**: List templates
- **list_traces**: List execution traces
- **list_workflows**: List workflows
- **run_workflow_with_contact**: Run workflow for contact
- **run_workflow**: Run AI workflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SketricGen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run my customer support agent workflow in SketricGen with the question 'How do I reset my password?'"

**🤖 AI Agent:**
> I've successfully triggered the customer support workflow. The agent accessed the 'Password Reset Guide' from your knowledge base and generated a step-by-step response. Would you like me to send this reply to the user?

---

**👤 You:**
> "Show me the execution trace and credit usage for my last SketricGen workflow run."

**🤖 AI Agent:**
> Retrieving the execution trace... Your last workflow completed in 4.2 seconds and consumed 15 credits. It successfully executed 3 tool calls and queried the main knowledge base once. Do you want to see the specific input and output for each node?

---

**👤 You:**
> "List all knowledge bases in SketricGen and show which agents are connected to each."

**🤖 AI Agent:**
> You have two active knowledge bases: 'Internal HR Docs' (connected to the HR Assistant agent) and 'Public FAQs' (connected to the Support Bot and Sales Bot). The 'Public FAQs' base currently contains 45 indexed documents.


## ❓ FAQ

**Q: How can my AI analyze the execution steps of a specific workflow?**
Simply use the `debug_workflow_trace` tool. Your agent will instantly retrieve the execution trace, detailing every tool call, data transfer between agents, and total credit consumption per run.

**Q: Is it possible to programmatically manage and query documents for my agents?**
Yes. By executing the `manage_knowledge_base` action, your AI agent can upload files (PDF, DOCX, TXT, HTML) or search existing repositories to provide context-aware, highly accurate responses.

**Q: Can I automatically trigger workflows tied to specific customer records?**
Absolutely. Ask the agent to use the `run_workflow_for_contact` tool. It will execute the designated workflow while injecting the specific contact's history, enabling personalized, data-driven outputs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sketricgen](https://vinkius.com/mcp/sketricgen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SketricGen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sketricgen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SketricGen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sketricgen": {
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
