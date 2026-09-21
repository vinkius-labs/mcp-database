# Sneaker Size Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sneaker-size-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Translate footwear sizes across US, UK, EU, JP, and CM systems.

## Description
This MCP server provides precise footwear sizing translations between global standards. Use `get_equivalent_sizes` to find matching sizes in different systems, or `get_size_from_length` to determine the best fit from a physical centimeter measurement. It also includes `get_size_range_info` for technical footprint details and `validate_measurement_completeness` to ensure input accuracy.


## Available Tools (4)
- **get_equivalent_sizes**: Finds the equivalent sizes in all supported systems for a given measurement or size
- **get_size_from_length**: Determines the appropriate shoe size based on a raw foot length measurement
- **get_size_range_info**: Provides technical details about a specific size's physical footprint
- **validate_measurement_completeness**: Checks if the provided input is sufficient to perform a reliable conversion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sneaker Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is a US size 10 equivalent in EU and UK?"

**🤖 AI Agent:**
> A US size 10 is equivalent to an EU 44 and a UK 9.

---

**👤 You:**
> "My foot is 26.5cm long. What shoe size should I get?"

**🤖 AI Agent:**
> Based on a 26.5cm measurement, the appropriate size is US 8.5 (EU 42, UK 7.5, JP 26.5). Please check the specific brand's size chart for the best fit.

---

**👤 You:**
> "What is the physical footprint of a UK size 7?"

**🤖 AI Agent:**
> A UK size 7 covers a foot length interval of 25.5cm to 26.0cm.


## ❓ FAQ

**Q: How accurate are these conversions?**
Conversions use verified sizing tables. However, because brands have proprietary charts, the tool will suggest checking a brand-specific chart for a perfect fit.

**Q: Can I convert from a physical foot measurement?**
Yes, you can use `get_size_from_length` by providing your foot length in centimeters.

**Q: What sizing systems are supported?**
The server supports US, UK, EU, JP, and CM (centimeter) systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sneaker-size-converter](https://vinkius.com/en/ai-agent-connect/sneaker-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sneaker Size Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sneaker-size-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sneaker Size Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sneaker-size-converter": {
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
