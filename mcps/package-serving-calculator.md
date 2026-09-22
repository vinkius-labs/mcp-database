# Package Serving Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/package-serving-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate total, full, and remaining servings from package weight.

## Description
This MCP server provides precise tools for nutritional and packaging analysis. Use `getTotalServings` to find the exact mathematical servings, `getFullServings` to determine the count of whole portions, and `getServingRemainder` to find the leftover weight. It also includes `validateServingRatio` to ensure serving sizes are logically consistent with the total package weight.


## Available Tools (4)
- **getFullServings**: Calculate whole servings
- **getServingRemainder**: Calculate leftover weight
- **getTotalServings**: Calculate total mathematical servings
- **validateServingRatio**: Validate serving plausibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Package Serving Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many full servings are in a 500g package if the serving size is 45g?"

**🤖 AI Agent:**
> There are 11 full servings in a 500g package with a 45g serving size.

---

**👤 You:**
> "What is the exact mathematical number of servings for 100g with a 30g serving size?"

**🤖 AI Agent:**
> The total number of servings is 3.3333333333333335.

---

**👤 You:**
> "Calculate the leftover weight for a 250g package with a 60g serving size."

**🤖 AI Agent:**
> The leftover weight is 10g.


## ❓ FAQ

**Q: How do I calculate the number of whole servings?**
You can use the `getFullServings` tool to get the count of complete, whole servings by providing the package weight and the serving size.

**Q: Can I check if a serving size is valid for a package?**
Yes, the `validateServingRatio` tool checks if the serving size is physically plausible relative to the total package weight.

**Q: What happens if there is leftover weight?**
You can use `getServingRemainder` to calculate the exact weight of the leftover portion that does not make up a full serving.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/package-serving-calculator](https://vinkius.com/en/ai-agent-connect/package-serving-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Package Serving Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `package-serving-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Package Serving Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "package-serving-calculator": {
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
