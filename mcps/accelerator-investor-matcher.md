# Accelerator Investor Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-investor-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluates alignment between startups and investors to find optimal funding matches.

## Description
This MCP server provides a specialized matching engine that evaluates the alignment between startup profiles and accelerator investor profiles. It calculates match scores, investor fit rankings, and introduction priorities by analyzing sector, stage, geography, and funding needs against investor theses. Use `find_investor_matches` to identify potential partners, `check_portfolio_conflicts` to avoid direct competitors, and `get_investor_capacity` to ensure investors have sufficient unallocated capital for the requested amount.


## Available Tools (3)
- **get_investor_capacity**: Checks if an investor has remaining capital availability to meet a startup's funding need
- **check_portfolio_conflicts**: Determines if a specific investor has a direct conflict of interest with a startup
- **find_investor_matches**: Identifies and ranks all investors that align with a specific startup's profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Investor Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me investors for a Fintech startup in the Seed stage located in Europe needing $2M."

**🤖 AI Agent:**
> I have found 3 matching investors. Global Ventures has a match score of 95 and is ranked as a High priority introduction.

---

**👤 You:**
> "Does Investor ID 'inv_123' have any conflicts with a Cybersecurity startup?"

**🤖 AI Agent:**
> No, there are no direct portfolio conflicts for 'inv_123' in the Cybersecurity sector.

---

**👤 You:**
> "Check if 'accel_99' can fund a $500,000 request."

**🤖 AI Agent:**
> Yes, 'accel_99' has sufficient remaining capacity to meet the $500,000 funding requirement.


## ❓ FAQ

**Q: How is the match score calculated?**
The score is determined by the density of overlaps between the startup's profile (sector, stage, geography) and the investor's strategic thesis.

**Q: What happens if an investor has a portfolio conflict?**
If `check_portfolio_conflicts` identifies a company in the same sector, the match score is significantly penalized or nullified to prevent conflicts of interest.

**Q: Can I check if an investor has enough money for my startup?**
Yes, you can use `get_investor_capacity` to verify if an investor's remaining unallocated capital meets your specific funding need.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-investor-matcher](https://vinkius.com/ai-agent-connect/accelerator-investor-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Investor Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-investor-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Investor Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-investor-matcher": {
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
