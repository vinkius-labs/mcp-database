# Handmade Gift Commission Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/handmade-gift-commission-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Transform raw gift ideas into structured creative briefs and logistical handoff plans.

## Description
This MCP server acts as a specialized planning engine for custom gift commissions. It bridges the gap between a user's abstract inspiration and an artisan's execution by generating professional creative briefs, approval checklists, and delivery logistics. Use `generate_creative_brief` to define the vision, `formulate_approval_questions` to confirm details with the contact, `finalize_making_commitments` to set artisan expectations, and `plan_presentation_and_handoff` to organize the final reveal and delivery.


## Available Tools (4)
- **finalize_making_commitments**: Generates a formal set of commitments that the artisan is expected to uphold
- **formulate_approval_questions**: Generates a checklist of questions to be answered by the approval contact to finalize the plan
- **generate_creative_brief**: Translates raw user inputs into a professional vision document for the artisan
- **plan_presentation_and_handoff**: Creates the final logistics for how the gift is presented and delivered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Handmade Gift Commission Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to commission a hand-knitted blue scarf for a birthday. The recipient loves soft textures and ocean themes."

**🤖 AI Agent:**
> Creative Brief: Ocean-inspired soft blue knitted scarf. Vision: A cozy, high-quality knit featuring soothing blue tones and textures reminiscent of sea foam. Personalization: Birthday gift.

---

**👤 You:**
> "Help me plan how to deliver a wooden jewelry box made via woodworking."

**🤖 AI Agent:**
> Presentation Plan: A slow reveal where the box is placed on a velvet cushion. Delivery Plan: Hand-delivered by a courier to ensure the delicate wood finish is preserved.

---

**👤 You:**
> "Generate approval questions for a custom leather wallet commission with a 2-week deadline."

**🤖 AI Agent:**
> 1. Does the proposed leather texture align with the desired aesthetic? 2. Is the 2-week deadline sufficient for the requested engraving? 3. Does the wallet size meet the user's functional requirements?


## ❓ FAQ

**Q: How does this server handle recipient privacy?**
The engine applies strict privacy and consent protocols, ensuring sensitive recipient data is only shared when absolutely necessary for the craft, or flagged for the approval contact.

**Q: Can I use this to plan a professional artisan commission?**
Yes, by using `finalize_making_commitments`, you create a formal operational roadmap that the artisan is expected to uphold.

**Q: What is the purpose of the presentation plan?**
The `plan_presentation_and_handoff` tool creates a strategy for the 'unboxing' or reveal, ensuring the gift's presentation aligns with the intended occasion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/handmade-gift-commission-plan](https://vinkius.com/en/ai-agent-connect/handmade-gift-commission-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Handmade Gift Commission Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `handmade-gift-commission-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Handmade Gift Commission Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "handmade-gift-commission-plan": {
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
