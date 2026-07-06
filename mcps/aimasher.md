# AiMasher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aimasher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate marketing content, social media posts, and creative assets using multiple AI models in a single unified workspace.

## Description
Connect your **AiMasher** account to any AI agent and take full control of your article rewriting orchestration and automated content blueprinting through natural conversation.

### What you can do

- **Campaign & Blueprint Orchestration** — List and manage your entire database of content campaigns programmatically, retrieving detailed platform metadata
- **Template Intelligence Architecture** — Programmatically retrieve your custom article rewriting templates to maintain a perfectly coordinated content strategy
- **Publishing & Feed Monitoring** — Access real-time updates for article blueprints and track publishing rules directly through your agent for instant reporting
- **Metadata Management** — Programmatically retrieve source URLs and author metadata to maintain a perfectly coordinated content record
- **Operational Monitoring** — Verify account-level API connectivity and monitor campaign query volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AiMasher dashboard (Profile > Get API Key)
3. Start orchestrating your content growth from Claude, Cursor, or any MCP client

No more manual copying of article blueprints or missing campaign updates. Your AI acts as your dedicated content coordinator and rewriting architect.

### Who is this for?

- **Content Marketers** — instantly retrieve campaign summaries and monitor article generation using natural language commands
- **Blogger & Site Owners** — verify individual template metadata and track publishing history without leaving your workspace
- **Developers** — integrate high-speed AiMasher data into custom RSS and autoblogging pipelines through simple AI queries


## Available Tools (10)
- **get_account**: Get account information
- **get_campaign**: Get campaign details
- **get_template**: Get template details
- **list_campaigns**: List all AI campaigns
- **list_outputs**: List campaign outputs
- **list_results**: List all generated results
- **list_templates**: List all content templates
- **check_aimasher_status**: Verify AIMasher API connectivity
- **create_campaign**: Optionally assign a template.

Create a new AI campaign
- **generate_content**: Optionally pass a custom prompt.

Generate content for a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AiMasher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my AiMasher account."

**🤖 AI Agent:**
> I've retrieved your campaigns. You currently have 5 active profiles, including 'Daily Tech Feed' and 'Marketing Blueprint'. Would you like the detailed platform metadata for any of them?

---

**👤 You:**
> "Show my article rewriting templates."

**🤖 AI Agent:**
> Template architecture orchestrated! I've identified 3 rewriting templates, including 'Professional Tone' and 'Creative Spin'. I've retrieved the technical metadata for your review. Need help selecting a template for your next campaign?

---

**👤 You:**
> "Check the status of my latest article blueprints."

**🤖 AI Agent:**
> Blueprint intelligence orchestrated! I've identified 10 article blueprints processed today. All are ready for your final publishing rules. Your API connection is healthy. Shall I retrieve the detailed word count metadata?


## ❓ FAQ

**Q: How do I find my AiMasher API Key?**
Log in to your account, click on your email address in the upper-right corner, and select **Get API Key** from the dropdown menu.

**Q: Can I retrieve rewriting templates via AI?**
Yes! The `list_templates` tool allows your agent to retrieve metadata for all your custom article blueprints.

**Q: How do I list my active campaigns?**
Use the `list_campaigns` tool to retrieve your complete directory along with the unique identifiers for all managed workstreams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aimasher](https://vinkius.com/mcp/aimasher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AiMasher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aimasher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AiMasher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aimasher": {
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
