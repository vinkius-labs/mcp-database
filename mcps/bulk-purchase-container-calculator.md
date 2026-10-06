# Bulk Purchase Container Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bulk-purchase-container-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculates required reusable containers based on product mass, density, and volume constraints.

## Description
This MCP server provides logistics optimization tools to determine the minimum number of reusable containers needed for bulk transport. It reconciles product mass and density against container volume and weight limits. Use `calculate_container_needs` to find total container counts, `check_compatibility` to verify if products can share space, `analyze_efficiency` to identify if a container is volume or weight constrained, and `group_by_separation_rules` to organize products into safe shipping groups.

### Available Tools

`calculate_container_needs_tool`, `check_compatibility_tool`, `analyze_efficiency_tool`, `group_by_separation_rules_tool`


## Available Tools (4)
- **calculate_container_needs_tool**: Determines the total number of containers required for a specific product order
- **check_compatibility_tool**: Verifies if two products can be safely stored within the same container
- **group_by_separation_rules_tool**: Organizes a list of multiple product quantities into distinct groups that can be shipped together
- **analyze_efficiency_tool**: Evaluates how well a specific container configuration uses its capacity for a given product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bulk Purchase Container Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many containers do I need for 500kg of product with a density of 0.5, using 100L containers that have a 200kg limit and a 90% fill limit?"

**🤖 AI Agent:**
> You will need 12 containers to transport this product.

---

**👤 You:**
> "Are 'Product_A' and 'Product_B' compatible for the same container?"

**🤖 AI Agent:**
> No, 'Product_A' and 'Product_B' are incompatible due to chemical reactivity constraints.

---

**👤 You:**
> "Is my container being limited by weight or volume for a product with 1000kg mass and 0.8 density in a 200L/500kg container?"

**🤖 AI Agent:**
> The container is Volume Constrained.


## ❓ FAQ

**Q: How does the tool determine the number of containers needed?**
The `calculate_container_needs` tool calculates the effective capacity by applying the fill limit to both volume and weight, then selects the most restrictive constraint based on the product's density. Tools available: `calculate_container_needs_tool`, `check_compatibility_tool`, `analyze_efficiency_tool`.

**Q: Can I check if two chemicals can be shipped together?**
Yes, use the `check_compatibility` tool to verify if two specific product identifiers are compatible according to established separation rules.

**Q: What is a fill limit?**
A fill limit is a safety buffer (e.g., 0.90 for 90%) applied to the container's volume and weight capacity to ensure containers are not filled to the absolute brim.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bulk-purchase-container-calculator](https://vinkius.com/en/ai-agent-connect/bulk-purchase-container-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bulk Purchase Container Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bulk-purchase-container-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bulk Purchase Container Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bulk-purchase-container-calculator": {
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
