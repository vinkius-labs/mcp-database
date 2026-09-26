# Creative Residency Decision Support MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-residency-decision-support)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Evaluate creative residency opportunities against your personal goals and constraints.

## Description
This MCP server provides a decision-support engine for artists and creatives. It helps you determine whether to apply, decline, or defer a residency by weighing host terms against your specific goals, costs, and accessibility needs. Use `evaluate_residency_options` to get a primary decision, `generate_application_strategy` to build a pursuit plan, `formulate_host_inquiries` to resolve uncertainties, `create_commitment_plan` to manage existing obligations, and `draft_contingency_arrangement` to prepare for potential risks.


## Available Tools (5)
- **draft_contingency_arrangement**: Create a "Plan B" based on the primary decision and potential risks
- **evaluate_residency_options**: Determine the primary decision (Apply, Decline, or Defer) for a specific residency option
- **generate_application_strategy**: Provide specific actions required to pursue a residency marked as "Apply" or "Defer"
- **create_commitment_plan**: Outline how the user will balance the residency with their existing life and work
- **formulate_host_inquiries**: Generate a list of questions for the residency organizers to resolve "Defer" states


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Residency Decision Support** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I apply for the Summer Arts Residency? It costs $2000 and provides a studio, but I have a work commitment in July."

**🤖 AI Agent:**
> The decision is Defer. While the studio meets your goals, the July work commitment creates a scheduling conflict that needs to be resolved with the host first.

---

**👤 You:**
> "I want to apply for the Mountain Retreat. Help me plan my application."

**🤖 AI Agent:**
> To pursue the Mountain Retreat, you should first finalize your portfolio, draft your project statement focusing on nature-inspired work, and prepare your letters of recommendation.

---

**👤 You:**
> "What questions should I ask the host about accessibility?"

**🤖 AI Agent:**
> You should ask: 'Does the studio space have step-free access?' and 'Are there specific height-adjustable workstations available in the facility?'


## ❓ FAQ

**Q: How does the tool decide to 'Decline' a residency?**
A residency is automatically declined if it violates any of your mandatory terms, such as exceeding your maximum cost threshold or failing to meet specific accessibility requirements.

**Q: What is the difference between 'Defer' and 'Decline'?**
Decline means the residency is a non-starter due to hard constraints. Defer means the residency is interesting, but you need more information (like specific accessibility details) before you can commit.

**Q: Can I use this to manage my schedule?**
Yes, you can use `create_commitment_plan` to outline how you will balance your existing obligations with the residency timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-residency-decision-support](https://vinkius.com/en/ai-agent-connect/creative-residency-decision-support)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Residency Decision Support** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-residency-decision-support` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Residency Decision Support** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-residency-decision-support": {
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
