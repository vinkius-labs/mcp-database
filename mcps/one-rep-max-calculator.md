# One Rep Max Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/one-rep-max-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate your maximum lifting capacity using Epley, Brzycki, and Lander models.

## Description
This MCP server provides specialized tools for strength athletes to predict their One Repetition Maximum (1RM) without the physical strain of a true max test. Use `get_epley_estimate` for a widely recognized method, `get_brzycki_estimate` for an alternative approach based on intensity ratios, or `get_lander_estimate` for a more complex statistical model. You can also use `get_lift_intensity` to determine the training load percentage of your sets.


## Available Tools (4)
- **get_epley_estimate**: Determine the estimated 1RM using the Epley method
- **get_lift_intensity**: Calculate the percentage of a user's maximum capability used
- **get_lander_estimate**: Determine the estimated 1RM using the Lander/Lombardi method
- **get_brzycki_estimate**: Determine the estimated 1RM using the Brzycki method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **One Rep Max Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my estimated 1RM if I lifted 100kg for 5 reps using the Epley method?"

**🤖 AI Agent:**
> Using `get_epley_estimate`, your estimated 1RM is 125kg.

---

**👤 You:**
> "Calculate the intensity of a 80lb set if my max is 100lb."

**🤖 AI Agent:**
> The `get_lift_intensity` tool shows your training intensity was 80%.

---

**👤 You:**
> "Estimate my max using Brzycki with 200lbs for 3 reps."

**🤖 AI Agent:**
> The `get_brzyck_estimate` tool predicts a 1RM of approximately 210.53lbs.


## ❓ FAQ

**Q: What is 1RM?**
One Repetition Maximum (1RM) is the heaviest weight you can lift for a single repetition with proper form.

**Q: Which estimation model should I use?**
It depends on your preference. `get_epley_estimate` is standard, while `get_brzycki_estimate` and `get_lander_estimate` offer alternative mathematical approaches.

**Q: Can I calculate training intensity?**
Yes, use the `get_lift_intensity` tool to find out what percentage of your estimated 1RM you used during a set.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/one-rep-max-calculator](https://vinkius.com/mcp/one-rep-max-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **One Rep Max Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `one-rep-max-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **One Rep Max Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "one-rep-max-calculator": {
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
