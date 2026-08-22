# Career Progression Timeline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/career-progression-timeline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Project career velocity, promotion age, and 10-year salary growth for Singapore professionals.

## Description
This MCP server provides deterministic career modeling for professionals in Singapore. It calculates the remaining years until your next promotion and your projected age at that milestone using `calculate_promotion_timeline`. You can also estimate future earnings using `project_salary_growth` to see how promotions and annual raises compound over a decade. For sector-specific rules, use `get_industry_benchmarks` to see how tech, finance, or consulting affects your career speed.


## Available Tools (3)
- **calculate_promotion_timeline**: Calculate the remaining years to the next promotion and the expected age at that milestone
- **get_industry_benchmarks**: Retrieve industry-specific progression offsets and baseline durations
- **project_salary_growth**: Project salary growth after the next promotion and over a 10-year period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Career Progression Timeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a junior in tech, 25 years old, and have been in this role for 1 year. When will I be mid-level?"

**🤖 AI Agent:**
> You will reach the mid-level in 1.5 years, at the age of 26.5.

---

**👤 You:**
> "My current salary is 80000. How much will I earn after my next promotion and what will my salary be in 10 years?"

**🤖 AI Agent:**
> After your next promotion, your salary will be 100000. In 10 years, your projected annual salary will be 161270.

---

**👤 You:**
> "What are the standard progression rules for the finance industry?"

**🤖 AI Agent:**
> In finance, the adjustment offset is 0 years, meaning progression follows the standard baseline durations for all levels.


## ❓ FAQ

**Q: How are industry adjustments calculated?**
The tool applies specific offsets to baseline progression durations: Tech subtracts 0.5 years, Finance is the baseline (0 years), and Consulting subtracts 1 year.

**Q: Can I project my salary after a promotion?**
Yes, by using `project_salary_growth`, you can see your immediate salary after a promotion and your projected annual salary after 10 years of compounding growth.

**Q: What career levels are supported?**
The model supports entry, junior, mid, senior, and lead levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/career-progression-timeline](https://vinkius.com/ai-agent-connect/career-progression-timeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Career Progression Timeline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `career-progression-timeline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Career Progression Timeline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "career-progression-timeline": {
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
