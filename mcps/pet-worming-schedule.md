# Pet Worming Schedule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-worming-schedule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Calculate deworming intervals and product suitability for dogs and cats based on age and risk.

## Description
This MCP server provides a specialized calculator for canine and feline deworming protocols. By analyzing species, age in months, and environmental exposure risk, it determines the recommended frequency of treatments. Use `deworming_interval_tool` to find optimal intervals, `product_suitability_tool` to verify if medications like PuppyGuard are appropriate, and `milestones_tool` to track upcoming lifecycle transitions.


## Available Tools (3)
- **milestones_tool**: Get upcoming deworming milestones
- **deworming_interval_tool**: Calculate the recommended deworming interval
- **product_suitability_tool**: Check if a deworming product is suitable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Worming Schedule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recommended deworming frequency for a 2-month-old puppy with high exposure risk?"

**🤖 AI Agent:**
> For a 2-month-old puppy with high exposure risk, the recommended interval is every 4 weeks to ensure protection during this critical growth phase.

---

**👤 You:**
> "Is PuppyGuard suitable for a 12-month-old cat?"

**🤖 AI Agent:**
> Yes, PuppyGuard is suitable for a 12-month-old cat, but note that it is optimized for the infant stage.

---

**👤 You:**
> "What are the upcoming deworming milestones for my 6-month-old dog?"

**🤖 AI Agent:**
> Your dog is approaching a transition phase. The next milestone is the shift from the intensive puppy protocol to the adult maintenance schedule.


## ❓ FAQ

**Q: How does the interval calculation work?**
The tool uses `deworming_interval_tool` to evaluate the pet's age and exposure risk. Puppies and kittens receive more frequent doses, while adults follow schedules based on their environmental contact level.

**Q: Can I check if a specific medication is safe?**
Yes, use the `product_suitability_tool` to verify if products like PuppyGuard or AdultShield are appropriate for your pet's current species and age.

**Q: What information is needed for the milestones tool?**
The `milestones_tool` requires only the species and the pet's current age in months to identify upcoming deworming transitions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-worming-schedule](https://vinkius.com/mcp/pet-worming-schedule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Worming Schedule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-worming-schedule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Worming Schedule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-worming-schedule": {
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
