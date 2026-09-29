# Repair & Disposal Decision Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-disposal-decision-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Evaluates the most responsible next steps for physical items based on condition, cost, and environmental impact.

## Description
This MCP server provides a decision-support engine to determine whether to repair, reuse, recycle, or replace physical items. By analyzing item condition and technical feasibility with `analyze_repair_feasibility`, comparing costs via `evaluate_economic_viability`, and identifying sustainable end-of-life paths through `select_disposal_path`, it generates a cohesive, responsible action plan using `generate_final_plan`. It helps users balance economic constraints with environmental responsibility.


## Available Tools (4)
- **analyze_repair_feasibility**: Determines if an item can realistically be fixed given its current state and technical report
- **evaluate_economic_viability**: Compares the cost of repairing the item against the cost of replacing it
- **generate_final_plan**: Aggregates all previous evaluations into a single, cohesive next-step plan
- **select_disposal_path**: Identifies the best way to handle an item that cannot be repaired or is being replaced


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair & Disposal Decision Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My laptop has a cracked screen. The repair costs $150, a new one is $800, and my budget is $200. Is it worth fixing?"

**🤖 AI Agent:**
> Yes, repairing the laptop is the most responsible and economically sound choice as the $150 cost is within your $200 budget and significantly lower than the $800 replacement cost.

---

**👤 You:**
> "I have an old broken toaster that cannot be fixed. How should I get rid of it?"

**🤖 AI Agent:**
> Since the item is non-functional, you should use specialized waste collection or local recycling services to ensure the components are handled responsibly.

---

**👤 You:**
> "I have a functional wooden chair that is slightly scratched. What should I do?"

**🤖 AI Agent:**
> Since the chair is functional, the most sustainable path is to donate it or find a way to reuse it, extending its life before considering recycling.


## ❓ FAQ

**Q: How does the engine decide between repair and replacement?**
The engine uses `evaluate_economic_viability` to compare the cost of repair against the cost of a new replacement and the user's budget to find the most sensible path.

**Q: Can I use this for electronic waste?**
Yes. By using `select_disposal_path`, the engine identifies specialized collection or recycling methods for hazardous categories like electronics.

**Q: What information do I need to provide?**
You should provide the item's condition, a technical repairability report, estimated costs, and any local disposal regulations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-disposal-decision-engine](https://vinkius.com/en/ai-agent-connect/repair-disposal-decision-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair & Disposal Decision Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-disposal-decision-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair & Disposal Decision Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-disposal-decision-engine": {
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
