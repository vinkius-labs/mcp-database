# Happierleads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/happierleads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Connect Happierleads to any AI agent via MCP.



## Available Tools (1)
- **happierleads_info**: Get information from Happierleads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Happierleads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show recent website visitors from the software industry."

**🤖 AI Agent:**
> I found 12 companies in the software industry that visited your site in the last 24 hours. The top visitors by page views are Acme Corp, Beta Software, and Cloud Solutions Inc.

---

**👤 You:**
> "Find contact details for decision makers at Acme Corp."

**🤖 AI Agent:**
> Here are the top decision makers at Acme Corp: 
1. John Doe (CEO) - john.doe@acme.com
2. Jane Smith (VP of Marketing) - jane.smith@acme.com

---

**👤 You:**
> "Summarize today's lead activity."

**🤖 AI Agent:**
> Today, your website received 150 unique B2B visitors. 45 matches were identified, with 12 highly engaged accounts viewing pricing pages. I recommend prioritizing outreach to AlphaTech and ZetaData.


## ❓ FAQ

**Q: What is Happierleads?**
Happierleads is a B2B website visitor identification tool that reveals which companies are visiting your website and provides contact details for decision makers.

**Q: Where do I find my API key?**
You can generate and access your API key in the Happierleads dashboard under your Account Settings or Developer settings.

**Q: Can I filter visitors by industry or company size?**
Yes, you can easily query and filter your website visitors by various attributes including industry, country, and employee count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/happierleads](https://vinkius.com/mcp/happierleads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Happierleads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `happierleads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Happierleads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "happierleads": {
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
