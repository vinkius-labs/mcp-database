# Seimei Handan Fortune Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/seimei-handan-fortune-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate Japanese name destiny using the Five Grids numerology.

## Description
This MCP server provides deterministic Japanese name fortune-telling (Seimei Handan) by calculating the Five Grids (Go-Grid) based on Kanji stroke counts. It allows AI agents to determine the auspiciousness of Heaven, Earth, Person, Outer, and Total grids using traditional numerology scales. Use `generate_full_report` to get a complete destiny summary or `evaluate_fortune` to check specific scores.


## Available Tools (3)
- **generate_full_report**: Generate a full fortune report
- **calculate_five_grids**: 
- **evaluate_fortune**: Evaluate if a score is auspicious


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seimei Handan Fortune Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fortune for a name with 10 family name strokes and 5 given name strokes using the modern method."

**🤖 AI Agent:**
> The Heaven score is 11 (Auspicious), the Earth score is 5 (Auspicious), the Person score is 15 (Auspicious), the Outer score is 6 (Auspicious), and the Total score is 37 (Auspicious).

---

**👤 You:**
> "Is a score of 12 considered lucky in Seimei Handan?"

**🤖 AI Agent:**
> No, a score of 12 is considered inauspicious.

---

**👤 You:**
> "Generate a full report for a name with 15 family strokes and 10 given strokes using Kangxi method."

**🤖 AI Agent:**
> The destiny analysis shows a Heaven score of 16, Earth of 10, Person of 25, Outer of 6, and a Total score of 57. The overall fortune is determined by these specific grid values.


## ❓ FAQ

**Q: What are the Five Grids?**
The Five Grids are Heaven, Earth, Person, Outer, and Total scores derived from Kanji stroke counts that represent different aspects of life.

**Q: What is the difference between Kangxi and Modern methods?**
Traditional Kangxi uses classical dictionary stroke counts, while Modern Japanese uses contemporary writing standards.

**Q: How do I get a complete analysis?**
You can use the `generate_full_report` tool to receive a comprehensive summary of all destiny scores and their auspiciousness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/seimei-handan-fortune-engine](https://vinkius.com/ai-agent-connect/seimei-handan-fortune-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seimei Handan Fortune Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seimei-handan-fortune-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seimei Handan Fortune Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seimei-handan-fortune-engine": {
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
