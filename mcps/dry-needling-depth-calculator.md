# Dry Needling Depth Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dry-needling-depth-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculates safe needle insertion parameters for trigger point therapy.

## Description
This MCP server provides clinical decision support for dry needling practitioners. It calculates precise needle length, insertion depth, and entry angles based on muscle thickness, target depth, and patient habitus. Use `get_insertion_parameters` to determine specific measurements, `validate_safety_boundaries` to check for neurovascular risks, `calculate_needle_selection` to find appropriate needle sizes, and `get_anatomical_constraints` to adjust for specific anatomical contexts like being near bone or nerves.


## Available Tools (4)
- **calculate_needle_selection**: Suggests the appropriate physical needle size (length) based on calculated requirements
- **get_anatomical_constraints**: Provides safety margin adjustments and angle limits based on anatomical risk categories
- **get_insertion_parameters**: Calculates the specific needle length, target insertion depth, and the required entry angle for a specific trigger point
- **validate_safety_boundaries**: Checks if a proposed needle insertion is safe given the anatomical constraints and patient profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dry Needling Depth Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate needle parameters for a muscle that is 30mm thick with a trigger point at 15mm depth for an average patient."

**🤖 AI Agent:**
> The required needle length is 22.5mm, the target insertion depth is 14.0mm, and the recommended entry angle is 90 degrees.

---

**👤 You:**
> "Is it safe to insert a needle 20mm deep in a 25mm thick muscle if there is a nerve nearby?"

**🤖 AI Agent:**
> No, the insertion is not safe. Due to the proximity to a vital structure, the risk level is high and a larger safety margin is required.

---

**👤 You:**
> "What is the best needle size for a required length of 28mm?"

**🤖 AI Agent:**
> The suggested needle size is 30mm.


## ❓ FAQ

**Q: How does the tool ensure needle safety?**
The tool uses `validate_safety_boundaries` to evaluate risks based on muscle thickness and proximity to vital structures, ensuring a mandatory safety margin is applied.

**Q: Can I adjust the angle of approach?**
Yes, you can specify a preferred angle using `get_insertion_parameters` to better suit the specific anatomical site.

**Q: What happens if a vital structure is nearby?**
If you indicate proximity to a vital structure, the tool increases the safety margin and provides stricter constraints to prevent injury.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dry-needling-depth-calculator](https://vinkius.com/en/ai-agent-connect/dry-needling-depth-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dry Needling Depth Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dry-needling-depth-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dry Needling Depth Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dry-needling-depth-calculator": {
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
