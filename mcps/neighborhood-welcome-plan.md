# Neighborhood Welcome Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/neighborhood-welcome-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [onboarding](../categories/onboarding.md)

Generates personalized community integration strategies and welcome packages for new residents.

## Description
This MCP server provides a complete toolkit for community leaders to welcome new residents. It uses `get_welcome_package` to create a full onboarding plan, `get_introduction_messages` for tailored outreach, `get_curated_resources` to find accessible local amenities, and `get_follow_up_timeline` to schedule meaningful touchpoints. All plans strictly respect resident privacy, accessibility needs, and budget constraints.


## Available Tools (4)
- **get_curated_resources**: 
- **get_follow_up_timeline**: 
- **get_introduction_messages**: 
- **get_welcome_package**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neighborhood Welcome Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a welcome package for a new resident named Alex who has mobility issues and loves parks."

**🤖 AI Agent:**
> The welcome package for Alex includes a greeting message, a list of accessible parks with paved walking paths, and a follow-up schedule focused on low-impact community events.

---

**👤 You:**
> "Create introduction messages for Sarah, but only via email."

**🤖 AI Agent:**
> Subject: Welcome to the neighborhood, Sarah!

Hi Sarah, we are so excited to have you join our community. We've put together some local resources to help you settle in.

---

**👤 You:**
> "What local resources are available for someone interested in fitness?"

**🤖 AI Agent:**
> Available resources include the Downtown Community Gym, the Riverside Running Trail, and the Westside Yoga Studio.


## ❓ FAQ

**Q: How does the server handle resident privacy?**
The server follows a strict Opt-in Contact Principle. No contact is initiated unless the resident explicitly grants permission via `contactPermissions`.

**Q: Can the welcome package be tailored to accessibility needs?**
Yes. By using `get_curated_resources`, the server filters local amenities to ensure they meet the resident's specific mobility, sensory, or language requirements.

**Q: Does the plan respect my budget?**
Yes. The `get_welcome_package` tool ensures that all suggested physical or premium digital materials stay within the user-provided budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/neighborhood-welcome-plan](https://vinkius.com/en/ai-agent-connect/neighborhood-welcome-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neighborhood Welcome Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neighborhood-welcome-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neighborhood Welcome Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neighborhood-welcome-plan": {
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
