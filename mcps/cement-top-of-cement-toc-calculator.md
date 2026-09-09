# Cement Top of Cement (TOC) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cement-top-of-cement-toc-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate Top of Cement (TOC) depth, displacement volumes, and annular capacity.

## Description
This MCP server provides specialized engineering tools for wellbore operations. It allows AI agents to determine the Top of Cement (TOC) depth by accounting for hole size, casing diameter, slurry volume, washout, and formation losses. Users can also calculate displacement requirements to move cement to target depths, determine bottom fill volumes, and compute annular capacity per unit length.


## Available Tools (4)
- **calculate_annular_capacity**: Provides the volume per unit of depth for a specific section of the well
- **calculate_bottom_fill**: Determines the volume of material occupying the bottom of the wellbore
- **calculate_displacement_requirements**: Calculates how much fluid is needed to move the cement to its target position
- **calculate_toc_depth**: Determines the depth at which the cement surface reaches within the wellbore


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cement Top of Cement (TOC) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the TOC depth for a 12-inch hole with 9.625-inch casing, 100 cubic feet of slurry, and 5% washout."

**🤖 AI Agent:**
> The calculated Top of Cement (TOC) depth is 450.25 feet.

---

**👤 You:**
> "How much fluid is needed to displace cement to a target TOC of 500 feet in a 12-inch hole with 9.625-inch casing?"

**🤖 AI Agent:**
> The required displacement volume is 125.4 cubic feet.

---

**👤 You:**
> "What is the volume of 10 feet of fill in a 12-inch hole?"

**🤖 AI Agent:**
> The fill volume for 10 feet of material in a 12-inch hole is 7.85 cubic feet.


## ❓ FAQ

**Q: How does washout affect the TOC calculation?**
Washout increases the effective hole diameter, which increases the annular volume and results in a different `calculate_toc_depth` result compared to a perfect cylinder.

**Q: Can I account for cement lost to the formation?**
Yes, the `calculate_toc_depth` tool includes an optional parameter for losses to adjust the effective slurry volume.

**Q: What is displacement volume?**
Displacement volume is the amount of fluid needed to push the cement to its target depth, which can be calculated using `calculate_displacement_requirements`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cement-top-of-cement-toc-calculator](https://vinkius.com/ai-agent-connect/cement-top-of-cement-toc-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cement Top of Cement (TOC) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cement-top-of-cement-toc-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cement Top of Cement (TOC) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cement-top-of-cement-toc-calculator": {
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
