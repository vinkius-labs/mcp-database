# Shoe Size Difference Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shoe-size-difference-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate the physical millimeter difference between any two shoe sizes across global standards.

## Description
This MCP server provides precise tools to bridge the gap between international shoe sizing systems. By converting various regional sizes into a unified physical length in millimeters, it allows for accurate comparisons between different standards. Use `calculate_size_gap` to find the physical difference between two specific shoes, `compare_standard_scales` to find an equivalent size in a different region, or `find_closest_size` to match a physical measurement to a standard size.


## Available Tools (4)
- **calculate_size_gap**: Determines the absolute physical difference between two different shoe sizes
- **compare_standard_scales**: Answers how much a size in one region differs from a size in another region for the same person
- **find_closest_size**: Identifies which standard size most closely matches a specific physical length
- **get_physical_length**: Converts a specific shoe size declaration into its equivalent physical foot length


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shoe Size Difference Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the physical difference between a US men's size 10 and a UK men's size 9?"

**🤖 AI Agent:**
> The physical difference between a US men's size 10 and a UK men's size 9 is 0 mm.

---

**👤 You:**
> "If my foot is 265mm long, what is my closest EU shoe size for women?"

**🤖 AI Agent:**
> The closest EU size for a 265mm foot is size 42.

---

**👤 You:**
> "Convert a US women's size 7 to an EU size."

**🤖 AI Agent:**
> A US women's size 7 is equivalent to an EU size 37.5.


## ❓ FAQ

**Q: How do I compare a US size to a UK size?**
You can use the `compare_standard_scales` tool to find the equivalent size in the UK for a given US size.

**Q: Can I calculate the difference between men's and women's sizes?**
Yes, by using `calculate_size_gap` and specifying the gender for each size, the tool calculates the absolute physical difference in millimeters.

**Q: What is the output format of the measurements?**
All physical measurements are returned in millimeters (mm) to ensure precision across all sizing systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shoe-size-difference-calculator](https://vinkius.com/en/ai-agent-connect/shoe-size-difference-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shoe Size Difference Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shoe-size-difference-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shoe Size Difference Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shoe-size-difference-calculator": {
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
