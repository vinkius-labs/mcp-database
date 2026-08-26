# Dairy Freestall Dimension Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dairy-freestall-dimension-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise dairy stall dimensions and assess cow comfort based on breed and design.

## Description
This MCP server provides engineering tools for dairy producers to design optimal freestall housing. By inputting cow weight, breed, and preferred stall design, users can determine critical dimensions like stall width, length, and curb height. The tools use Midwest Plan Service standards to ensure cow comfort and minimize injury risk. Use `calculate_stall_dimensions` to get physical measurements, `estimate_stall_metrics` to predict herd efficiency, `assess_injury_risk` to evaluate safety, and `validate_layout_compliance` to ensure industry standard adherence.


## Available Tools (4)
- **assess_injury_risk**: Evaluates the physical risk to the cow based on the designed dimensions
- **calculate_stall_dimensions**: Determines the specific physical dimensions required for a single stall based on cow characteristics and design type
- **estimate_stall_metrics**: Predicts the efficiency and usage of the stall layout
- **validate_layout_compliance**: Checks if a proposed stall configuration meets the minimum Midwest Plan Service standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dairy Freestall Dimension Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stall dimensions for a 1500lb Holstein using a loop design."

**🤖 AI Agent:**
> For a 1500lb Holstein with a loop design, the stall width is 48 inches, the length is 92 inches, the brisket locator is 34 inches from the curb, the neck rail height is 12 inches, and the curb height is 8 inches.

---

**👤 You:**
> "What is the injury risk for a 1200lb Jersey cow with a 10 inch neck rail height and 6 inch curb height?"

**🤖 AI Agent:**
> The injury risk level is Moderate, with the primary risk factor being the neck rail height.

---

**👤 You:**
> "Check if a 45 inch wide stall is compliant for a 1600lb Holstein."

**🤖 AI Agent:**
> The design is non-compliant. The width is 3 inches below the minimum standard. It is recommended to increase the stall width to at least 48 inches.


## ❓ FAQ

**Q: What standards are used for the calculations?**
All calculations and compliance checks are based on the Midwest Plan Service standards for dairy housing.

**Q: Can I calculate the risk of injury for my cows?**
Yes, you can use the `assess_injury_risk` tool to evaluate the risk level based on neck rail height, curb height, and cow weight.

**Q: Which breeds are supported?**
The tool currently supports Holstein and Jersey breeds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dairy-freestall-dimension-calculator](https://vinkius.com/ai-agent-connect/dairy-freestall-dimension-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dairy Freestall Dimension Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dairy-freestall-dimension-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dairy Freestall Dimension Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dairy-freestall-dimension-calculator": {
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
