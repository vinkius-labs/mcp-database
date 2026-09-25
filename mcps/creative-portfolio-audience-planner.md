# Creative Portfolio Audience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-portfolio-audience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Strategically map portfolio versions to target audiences and plan deployment.

## Description
This MCP server provides a strategic planning engine for creators. It automates the mapping of portfolio versions to specific target audiences using `get_audience_portfolio_mapping`. It also determines optimal hosting locations via `plan_publishing_actions`, identifies safe communication channels through `determine_contact_pathway`, and establishes management workflows with `define_operational_protocols`.


## Available Tools (4)
- **determine_contact_pathway**: Identifies valid ways to contact an audience while respecting privacy constraints
- **plan_publishing_actions**: Determines where and how to host portfolios based on available platforms and maintenance capacity
- **define_operational_protocols**: Establishes the ownership of updates and the procedure for handling responses
- **get_audience_portfolio_mapping**: Maps specific portfolio versions to target audiences based on priority and needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Portfolio Audience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Map my portfolios to these audiences: [{"id": "clients", "priority": "High"}] with needs: {"clients": ["photography", "design"]}."

**🤖 AI Agent:**
> The portfolio version containing 'photography' and 'design' has been mapped to your 'clients' audience.

---

**👤 You:**
> "Suggest platforms for my portfolios if I have Low maintenance capacity."

**🤖 AI Agent:**
> Based on your Low maintenance capacity, the recommended platform is a static landing page with automated updates.

---

**👤 You:**
> "What is the best way to contact an audience with strict privacy limits?"

**🤖 AI Agent:**
> The most appropriate method is using a contact form to ensure your direct contact details remain private.


## ❓ FAQ

**Q: How does the tool match my work to an audience?**
The `get_audience_portfolio_mapping` tool analyzes the work categories within your portfolio versions and compares them against the specific needs of your target audience to find the best fit.

**Q: Can I control how my contact information is shared?**
Yes. The `determine_contact_pathway` tool respects your privacy limits, ensuring that only contact methods matching your constraints are suggested.

**Q: How do I manage updates for different platforms?**
The `plan_publishing_actions` tool evaluates your maintenance capacity to recommend platforms that align with your ability to manage content updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-portfolio-audience-planner](https://vinkius.com/en/ai-agent-connect/creative-portfolio-audience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Portfolio Audience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-portfolio-audience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Portfolio Audience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-portfolio-audience-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
