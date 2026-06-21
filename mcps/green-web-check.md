# Green Web Check MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/green-web-check)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Universal sustainability intelligence — check if websites are hosted on green energy via AI.

## Description
Equip your AI agent with environmental intelligence through the **Green Web Foundation** MCP server. This integration provides instant verification of a website's hosting infrastructure. Your agent can check if a specific domain is powered by renewable energy sources based on the world's largest open database of green hosting. Whether you are auditing corporate sustainability, choosing eco-friendly vendors, or researching the environmental impact of the internet, your agent acts as a dedicated sustainability consultant through natural conversation.

### What you can do

- **Green Check** — Verify if any website URL is hosted on a platform using renewable energy.
- **Provider Insights** — Identify the hosting organization and access their official sustainability records.
- **Sustainability Auditing** — Run checks across multiple domains to profile your digital supply chain's carbon footprint.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start verifying website sustainability from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sustainability Officers** — audit the environmental impact of their organization's digital assets.
- **Eco-conscious Developers** — select hosting partners that align with green values.
- **Digital Ethics Researchers** — track the transition of the web toward renewable energy.
- **Procurement Teams** — verify the green claims of potential SaaS and cloud vendors.


## Available Tools
- **check_green_hosting**: Check if a website is hosted on green energy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Green Web Check** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if 'vinkius.com' is hosted on green energy."

**🤖 AI Agent:**
> Checking the Green Web Foundation database... I've verified that vinkius.com is indeed hosted on green energy. The provider is registered as using renewable sources for its infrastructure.

---

**👤 You:**
> "Is the hosting for 'amazon.com' environmentally friendly?"

**🤖 AI Agent:**
> Running a green check... amazon.com is hosted on AWS, which is registered as a green provider in many regions. I've confirmed that the specific infrastructure powering amazon.com is listed as green.

---

**👤 You:**
> "Which company hosts 'wikipedia.org' and is it green?"

**🤖 AI Agent:**
> Checking Wikipedia... wikipedia.org is hosted by the Wikimedia Foundation. According to the database, their hosting is currently powered by 100% renewable energy.


## ❓ FAQ

**Q: Is Google.com hosted on green energy?**
Yes! Google is a registered green hosting provider in the database. You can use the `check_green_hosting` tool to verify the status of any of its domains.

**Q: What does it mean if a site is not green?**
It means the hosting provider is either using conventional fossil-fuel-based energy or has not yet registered their renewable energy usage with the Green Web Foundation.

**Q: Can I check multiple domains in a single session?**
Yes. You can provide a list of domains to your AI agent, and it will call the `check_green_hosting` tool for each one, providing a summarized sustainability report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/green-web-check](https://vinkius.com/mcp/green-web-check)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Green Web Check** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `green-web-check` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Green Web Check** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "green-web-check": {
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
