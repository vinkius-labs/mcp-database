# Floor Flatness & Levelness Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/floor-flatness-levelness-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Analyze concrete floor compliance using FF/FL F-number standards.

## Description
This MCP server provides specialized tools for assessing concrete floor quality. It allows AI agents to determine if a surface meets specific flatness (FF) and levelness (FL) requirements using the F-number system. Users can use `analyze_f_number_compliance` to check if measurement points satisfy industry standards for various floor uses like warehouses or retail spaces. For non-compliant surfaces, `calculate_grinding_needs` provides estimates for corrective work. Additionally, `evaluate_straightedge_deviation` supports manual measurement analysis, and `get_classification_standards` retrieves default requirements for different floor classifications.


## Available Tools (4)
- **analyze_f_number_compliance**: 
- **calculate_grinding_needs**: 
- **evaluate_straightedge_deviation**: 
- **get_classification_standards**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Floor Flatness & Levelness Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these measurement points meet warehouse standards: points=[{'x':0,'y':0,'z':0.1},{'x':1,'y':1,'z':0.2}], area=50, use='warehouse', specs='{"minFF":25, "minFL":20}'"

**🤖 AI Agent:**
> The floor is non-compliant. The calculated FF is 22 and FL is 18, which are below the required warehouse standards of FF 25 and FL 20.

---

**👤 You:**
> "What are the standard FF and FL requirements for a High-Speed Warehouse?"

**🤖 AI Agent:**
> For a High-Speed Warehouse, the minimum requirements are FF 55 and FL 40.

---

**👤 You:**
> "Estimate the grinding needed for these non-compliant points: points=[{'x':0,'y':0,'z':0.5}], target={'targetZ':0.0}"

**🤖 AI Agent:**
> The estimated grinding depth is 0.5 meters covering an area of 1 square meter with a low complexity score.


## ❓ FAQ

**Q: What is the difference between FF and FL?**
FF (Floor Flatness) measures the waviness of the surface, while FL (Floor Levelness) measures the overall tilt or slope of the floor.

**Q: How can I check if my warehouse floor is compliant?**
You can use the `analyze_f_number_compliance` tool by providing your measurement points, the floor area, and the floor use classification.

**Q: Can I use manual straightedge measurements?**
Yes, the `evaluate_straightedge_deviation` tool is specifically designed to process manual gap measurements from a physical straightedge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/floor-flatness-levelness-analyzer](https://vinkius.com/ai-agent-connect/floor-flatness-levelness-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Floor Flatness & Levelness Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `floor-flatness-levelness-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Floor Flatness & Levelness Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "floor-flatness-levelness-analyzer": {
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
