# Social Profile Visibility Check MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/social-profile-visibility-check)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audit social media profiles against privacy policies to find exposure mismatches.

## Description
This MCP server provides tools to analyze social media profile configurations against a user's desired privacy policy. It identifies exposure mismatches where sensitive profile fields are visible to unauthorized audiences and suggests required setting changes. Use `analyze_profile_alignment` to perform a full audit, `get_audience_risk_level` to calculate a risk score, `validate_setting_change` to test proposed privacy adjustments, and `list_field_visibility_matrix` to see exactly who can view specific profile data.


## Available Tools (4)
- **analyze_profile_alignment**: Performs the core audit by comparing profile data and settings against a specific privacy policy
- **get_audience_risk_level**: Calculates a risk score based on the current profile configuration
- **list_field_visibility_matrix**: Provides a detailed breakdown of exactly who can see which specific profile fields
- **validate_setting_change**: Checks if a proposed change to a setting will successfully resolve an existing exposure mismatch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Profile Visibility Check** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my profile matches my privacy policy."

**🤖 AI Agent:**
> Your profile has 2 exposure mismatches: your birthdate is visible to the public, but your policy restricts it to friends only. You should change your account visibility to private.

---

**👤 You:**
> "What is my current privacy risk level?"

**🤖 AI Agent:**
> Your current risk level is High because your search visibility is set to public while your policy requires strict privacy.

---

**👤 You:**
> "Who can see my email address?"

**🤖 AI Agent:**
> Your email address is currently visible to all users due to your public profile setting.


## ❓ FAQ

**Q: How do I check if my profile is too public?**
You can use the `analyze_profile_alignment` tool by providing your current profile data and your desired privacy policy to identify any mismatches.

**Q: Can I test a privacy setting change before applying it?**
Yes, the `validate_setting_change` tool allows you to verify if a proposed setting adjustment will successfully resolve existing exposure mismatches.

**Q: What does the risk score represent?**
The risk score is a normalized value calculated by `get_audience_risk_level` that indicates your level of data exposure based on your current settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/social-profile-visibility-check](https://vinkius.com/en/ai-agent-connect/social-profile-visibility-check)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Profile Visibility Check** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-profile-visibility-check` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Profile Visibility Check** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-profile-visibility-check": {
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
