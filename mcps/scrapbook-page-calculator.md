# Scrapbook Page Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/scrapbook-page-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the total pages needed for your scrapbook projects.

## Description
This MCP server provides tools to plan your scrapbook projects accurately. It calculates the primary pages required for your photographs using `get_photo_page_requirement`, determines the grand total including journaling space with `get_total_scrapbook_plan`, validates if your layout density is practical via `validate_layout_density`, and suggests supplemental pages using `estimate_memory_needs`.


## Available Tools (4)
- **estimate_memory_needs**: Provides a recommendation for how many memory pages might be needed based on the number of photos
- **get_photo_page_requirement**: Determines how many pages are needed strictly to accommodate the planned photographs
- **get_total_scrapbook_plan**: Calculates the grand total of pages needed for a complete scrapbook
- **validate_layout_density**: Checks if a requested photo density is practical for a standard scrapbook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scrapbook Page Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many pages do I need for 50 photos if I put 4 photos on each page?"

**🤖 AI Agent:**
> You will need 13 primary pages for your 50 photos.

---

**👤 You:**
> "Calculate the total scrapbook plan for 30 photos, 5 photos per page, and 4 memory pages."

**🤖 AI Agent:**
> Your total scrapbook plan requires 10 pages: 6 primary pages for photos and 4 memory pages.

---

**👤 You:**
> "Is it practical to put 15 photos on one scrapbook page?"

**🤖 AI Agent:**
> No, a density of 15 photos per page is considered a very crowded layout.


## ❓ FAQ

**Q: How do I calculate the total pages for my scrapbook?**
You can use the `get_total_scrapbook_plan` tool, providing the number of photos, the density per page, and any extra memory pages you want to include.

**Q: Can I check if my photo layout is too crowded?**
Yes, use the `validate_layout_density` tool to check if your chosen number of photos per page is practical for a standard scrapbook.

**Q: How many memory pages should I add?**
The `estimate_memory_needs` tool can provide a recommendation based on your total photo count and your preferred photo-to-memory ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/scrapbook-page-calculator](https://vinkius.com/en/ai-agent-connect/scrapbook-page-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scrapbook Page Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scrapbook-page-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scrapbook Page Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scrapbook-page-calculator": {
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
