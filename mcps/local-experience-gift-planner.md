# Local Experience Gift Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-gift-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Plan perfect local gifts by matching recipient interests with available experiences and provider terms.

## Description
This MCP server helps you design thoughtful gift experiences. Use `query_experience_matches` to find activities within your budget, `validate_gift_feasibility` to ensure the recipient can participate based on their needs, and `generate_gift_proposal` to create a complete gift package including a message and redemption plan. It also includes `check_consent_compliance` to respect privacy boundaries.


## Available Tools (4)
- **generate_gift_proposal**: Assembles the final selection, message, and support plan
- **query_experience_matches**: Finds experiences that align with recipient interests and budget
- **validate_gift_feasibility**: Checks if a specific experience can be successfully gifted
- **check_consent_compliance**: Ensures the plan respects privacy boundaries and recipient consent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Gift Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me some culinary experiences in the city for under $100 for a birthday."

**🤖 AI Agent:**
> I found a Gourmet Coffee Tasting workshop for $45 and a Local Pastry Tour for $75. Both fit your $100 budget.

---

**👤 You:**
> "Can my recipient participate in a hiking tour if they use a mobility aid?"

**🤖 AI Agent:**
> The hiking tour requires significant walking and does not support mobility aids, so it is not a feasible option.

---

**👤 You:**
> "Create a gift proposal for Sarah for her graduation with a message: 'So proud of you!'"

**🤖 AI Agent:**
> Your gift proposal for Sarah is ready. The selected experience is the Botanical Garden Tour. Message: 'So proud of you!' Redemption: Show the digital voucher at the entrance.


## ❓ FAQ

**Q: How do I find experiences within my budget?**
You can use the `query_experience_matches` tool by providing the recipient's interests and your maximum spending cap.

**Q: Can I ensure the gift respects the recipient's privacy?**
Yes, the `check_consent_compliance` tool verifies that your proposed actions align with the defined privacy boundaries.

**Q: What happens if the chosen experience is not available?**
The `generate_gift_proposal` tool automatically includes a non-intrusive backup option that respects your original constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-gift-planner](https://vinkius.com/en/ai-agent-connect/local-experience-gift-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Gift Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-gift-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Gift Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-gift-planner": {
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
