# Ceramic Shrinkage & Glaze Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ceramic-shrinkage-glaze-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [tools](../categories/tools.md)

Calculate precise wet clay dimensions and glaze requirements for ceramic production.

## Description
This MCP server provides deterministic tools for ceramic artists and manufacturers to manage physical changes during the pottery process. Use `calculate_clay_dimensions` to determine the necessary wet size of a piece based on specific clay body shrinkage rates. Use `calculate_glaze_requirements` to find the exact mass of glaze needed for different application methods like dipping or spraying. Additionally, `get_firing_parameters` provides recommended bisque and glaze firing temperatures for porcelain, stoneware, earthenware, and raku clay bodies.


## Available Tools (3)
- **calculate_clay_dimensions**: Determines the necessary wet dimensions required to reach a specific target size after all shrinkage has occurred
- **calculate_glaze_requirements**: Calculates the mass of glaze needed and the ideal density for the specified application method
- **get_firing_parameters**: Provides the recommended temperature ranges for both the bisque and glaze firing stages based on the clay type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ceramic Shrinkage & Glaze Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What wet dimensions do I need for a porcelain piece that should be 10x10x10 cm, with 5% drying and 13% firing shrinkage?"

**🤖 AI Agent:**
> To achieve a finished size of 10x10x10 cm, your wet dimensions should be 11.9x11.9x11.9 cm based on a total shrinkage of 18%.

---

**👤 You:**
> "How much glaze do I need for a 500 sq cm surface using the dipping method?"

**🤖 AI Agent:**
> You will need 75 grams of glaze for a 500 sq cm surface using the dipping method.

---

**👤 You:**
> "What are the firing temperatures for earthenware?"

**🤖 AI Agent:**
> Earthenware typically requires a bisque firing around 1000°C and a glaze firing around 1050°C.


## ❓ FAQ

**Q: How do I calculate the wet size of my clay?**
You can use the `calculate_clay_dimensions` tool. Provide the clay type, your target finished dimensions, and the expected drying and firing shrinkage percentages.

**Q: Can I calculate glaze amounts for spraying?**
Yes, the `calculate_glaze_requirements` tool supports spraying, dipping, pouring, and brushing methods to determine the required glaze mass.

**Q: What firing temperatures are recommended for stoneware?**
You can retrieve specific temperature ranges for stoneware by using the `get_firing_parameters` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ceramic-shrinkage-glaze-calculator](https://vinkius.com/ai-agent-connect/ceramic-shrinkage-glaze-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ceramic Shrinkage & Glaze Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ceramic-shrinkage-glaze-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ceramic Shrinkage & Glaze Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ceramic-shrinkage-glaze-calculator": {
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
