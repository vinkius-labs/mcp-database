# TAM-SAM-SOM Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tam-sam-som-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Total Addressable Market (TAM), Serviceable Addressable Market (SAM), and Serviceable Obtainable Market (SOM) using top-down and bottom-up methodologies.

## Description
This MCP server provides a precise calculation engine for market sizing. By utilizing tools like `calculate_tam_base`, `apply_sam_refinement`, and `project_som_capture`, users can determine their total, reachable, and realistic market opportunities. The engine applies reduction filters (geographic and segment) to establish SAM from TAM, and projects Year 3 market share to arrive at SOM, providing a clear view of potential revenue and customer reach.


## Available Tools (3)
- **apply_sam_refinement**: Shrinks the initial TAM into a reachable SAM
- **calculate_tam_base**: Establies the initial baseline for the total market size
- **project_som_capture**: Determines the realistic market capture (SOM)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TAM-SAM-SOM Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my TAM if I have 50,000 potential customers and each spends $100 per year."

**🤖 AI Agent:**
> The Total Addressable Market (TAM) is $5,000,000 with 50,000 customers.

---

**👤 You:**
> "My TAM is $10M. If my geographic reach is 30% and my segment target is 50%, what is my SAM?"

**🤖 AI Agent:**
> Your Serviceable Addressable Market (SAM) is $1,500,000.

---

**👤 You:**
> "If my SAM is $2M and I expect to capture 5% of the market by year 3, what is my SOM?"

**🤖 AI Agent:**
> Your Serviceable Obtainable Market (SOM) is $100,000.


## ❓ FAQ

**Q: What is the difference between TAM, SAM, and SOM?**
TAM (Total Addressable Market) is the total global demand. SAM (Serviceable Addressable Market) is the portion reachable within your specific geography and segment. SOM (Serviceable Obtainable Market) is the realistic share you can capture by Year 3.

**Q: How do I start my calculation?**
Start by using the `calculate_tam_base` tool with either your total market revenue or your potential customer count and average revenue per user.

**Q: Can I apply geographic filters?**
Yes, use the `apply_sam_refinement` tool to apply a geographic reach ratio (e.g., 0.2 for 20% of the market) and segment target ratios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tam-sam-som-calculator](https://vinkius.com/mcp/tam-sam-som-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TAM-SAM-SOM Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tam-sam-som-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TAM-SAM-SOM Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tam-sam-som-calculator": {
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
