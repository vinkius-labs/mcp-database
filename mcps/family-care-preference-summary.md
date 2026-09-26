# Family Care Preference Summary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-care-preference-summary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Consolidate disparate caregiver inputs into a structured, actionable reference for care providers.

## Description
This MCP server transforms raw, unstructured caregiver data into a single source of truth. It organizes daily routines, dietary preferences, engagement activities, communication guides, comfort profiles, and strict boundaries into a structured format. Use `summarize_care_profile` to build a complete profile, `identify_critical_boundaries` to extract high-priority constraints, `generate_communication_guide` for interaction protocols, and `extract_comfort_and_environment` to identify soothing sensory needs.


## Available Tools (4)
- **extract_comfort_and_environment**: Extract information about comfort items and environmental needs to help soothe the person
- **generate_communication_guide**: Generate a guide on how to interact with the person to ensure they feel heard and understood
- **identify_critical_boundaries**: Identify the most important "do not" instructions to ensure safety and respect
- **summarize_care_profile**: Summarize care preferences from supplied routines, foods, activities, communication needs, comfort items, and explicit boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Care Preference Summary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize the care profile for a person who likes tea in the morning, needs quiet time after lunch, and must not be touched on their left arm."

**🤖 AI Agent:**
> Daily Routine: Prefers tea in the morning and quiet time after lunch. Dietary Preferences: Enjoys tea. Strict Boundaries: Do not touch the left arm.

---

**👤 You:**
> "What are the critical boundaries in this text: 'John loves music but hates loud noises. Do not play drums near him.'"

**🤖 AI Agent:**
> Do not play drums near him.

---

**👤 You:**
> "Create a communication guide for someone who responds well to soft tones and gentle gestures."

**🤖 AI Agent:**
> Verbal Style: Use soft tones. Non-Verbal Cues: Use gentle gestures.


## ❓ FAQ

**Q: Does this tool provide medical advice?**
No. This tool is strictly non-clinical and focuses on quality of life and person-centered care. It filters out medical instructions to focus on preferences.

**Q: How can I find the most important safety instructions?**
You can use the `identify_critical_boundaries` tool to extract high-priority 'do not' instructions from all provided care data.

**Q: Can I use this to create a communication plan?**
Yes, the `generate_communication_guide` tool creates a specific interaction protocol including verbal style and non-verbal cues.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-care-preference-summary](https://vinkius.com/en/ai-agent-connect/family-care-preference-summary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Care Preference Summary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-care-preference-summary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Care Preference Summary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-care-preference-summary": {
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
