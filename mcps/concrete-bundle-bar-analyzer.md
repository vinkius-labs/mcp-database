# Concrete Bundle Bar Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-bundle-bar-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Verify bundle bar compliance and spacing requirements using ACI provisions.

## Description
This MCP server provides structural engineering tools to analyze bundled reinforcement bars according to ACI standards. It calculates effective diameters, determines development length modification factors, and validates clear spacing to prevent concrete honeycombing. Engineers can use `check_bundle_compliance` to verify configuration safety, `calculate_development_length_modifier` for bond efficiency, `validate_spacing_requirements` for aggregate flow, and `evaluate_congestion_index` to assess reinforcement density.


## Available Tools (4)
- **check_bundle_compliance**: Determines if a specific bundle configuration meets ACI requirements for effective diameter and spacing
- **evaluate_congestion_index**: Quantifies how "crowded" a section of concrete is to alert the engineer to potential placement issues
- **validate_spacing_requirements**: Specifically checks if the gap between bundles or individual bars is wide enough for the specified concrete grade
- **calculate_development_length_modifier**: Computes the adjustment factor required for development length when using bundled bars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Bundle Bar Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a bundle of 4 bars with 20mm diameter is compliant with 30MPa concrete and 40mm clear spacing."

**🤖 AI Agent:**
> The bundle configuration is compliant. The effective diameter is 34.64mm and the required clear spacing is 35mm.

---

**👤 You:**
> "What is the development length modifier for 5 bars of 25mm diameter in a contact splice?"

**🤖 AI Agent:**
> The modification factor for this contact splice configuration is 0.72, resulting in an effective bond strength ratio of 0.72.

---

**👤 You:**
> "Is a 30mm gap sufficient for a 25mm bar with 20mm maximum aggregate size?"

**🤖 AI Agent:**
> Yes, the spacing is adequate for the specified aggregate size.


## ❓ FAQ

**Q: How does this tool handle bundled bars?**
The tool uses ACI provisions to calculate how bundled bars behave as a single unit, specifically adjusting for effective diameter and reduced bond strength.

**Q: Can I check for concrete congestion?**
Yes, you can use `evaluate_congestion_index` to quantify how crowded a section is and receive risk recommendations.

**Q: What is the purpose of the development length modifier?**
It computes the adjustment factor needed for development length to account for the reduced bond efficiency in bundled configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-bundle-bar-analyzer](https://vinkius.com/ai-agent-connect/concrete-bundle-bar-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Bundle Bar Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-bundle-bar-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Bundle Bar Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-bundle-bar-analyzer": {
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
