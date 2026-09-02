# Rebar Splice Decision Support MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rebar-splice-decision-support)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Evaluates rebar splicing methods based on structural, economic, and site constraints.

## Description
This MCP server provides a suite of engineering tools to compare rebar splicing alternatives. It calculates necessary lap splice lengths using `calculate_lap_splice_requirements`, estimates the financial impact via `estimate_mechanical_splice_cost`, and assesses site-specific viability with `evaluate_welded_splice_feasibility`. Finally, it uses `generate_splice_recommendation` to provide a data-driven decision between lap, mechanical, or welded splices based on congestion and cost.


## Available Tools (4)
- **evaluate_welded_splice_feasibility**: Determines if welding is a viable option based on site constraints and congestion
- **estimate_mechanical_splice_cost**: Calculates the total financial impact of using mechanical couplers
- **generate_splice_recommendation**: Provides a final decision by comparing all calculated factors
- **calculate_lap_splice_requirements**: Determines the necessary overlap length for a lap splice based on structural geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebar Splice Decision Support** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required lap splice length for a 25mm bar under tension at mid-span."

**🤖 AI Agent:**
> The required lap splice length for a 25mm bar under tension at mid-span is 1250mm.

---

**👤 You:**
> "Estimate the cost for 50 mechanical splices using 20mm diameter bars."

**🤖 AI Agent:**
> The total estimated cost for 50 mechanical splices with 20mm bars is $450.00.

---

**👤 You:**
> "Is welding feasible in a high congestion area with limited space?"

**🤖 AI Agent:**
> No, welding is not recommended in high congestion areas with limited space due to quality control risks.


## ❓ FAQ

**Q: How does the tool determine the lap splice length?**
The `calculate_lap_splice_requirements` tool determines the length based on the bar diameter, the type of load (tension or compression), and the structural zone location.

**Q: Can I use this to compare costs between methods?**
Yes. You can use `estimate_mechanical_splice_cost` to find the total cost of couplers and then use `generate_splice_recommendation` to compare that against other methods.

**Q: What factors influence the final recommendation?**
The recommendation is driven by the calculated lap length, the total mechanical cost, the feasibility of welding, and the reinforcement congestion level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rebar-splice-decision-support](https://vinkius.com/ai-agent-connect/rebar-splice-decision-support)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rebar Splice Decision Support** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rebar-splice-decision-support` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rebar Splice Decision Support** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rebar-splice-decision-support": {
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
