# Policy Change Impact Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/policy-change-impact-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Maps textual policy revisions to insured assets and planned activities to prevent coverage gaps.

## Description
This MCP server provides a specialized diagnostic suite for policyholders and insurers. It identifies textual deltas between policy versions using `analyze_policy_delta`, maps those changes to specific assets or activities via `map_impacts_to_entities`, and generates actionable verification steps with `generate_confirmation_checklist`. Additionally, use `validate_coverage_alignment` to detect if any assets or activities have become uncovered due to new wording.


## Available Tools (4)
- **analyze_policy_delta**: Identifies the specific changes made between the old and new policy versions
- **generate_confirmation_checklist**: Produces a final checklist of actionable statements for the user to verify their status
- **map_impacts_to_entities**: Determines which specific assets or activities are affected by the identified policy changes
- **validate_coverage_alignment**: A diagnostic tool to check if any specific asset or activity has become uncovered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Policy Change Impact Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two policy versions and tell me what changed."

**🤖 AI Agent:**
> The policy has been modified in the 'Exclusions' section. The age limit for mobile assets has been increased from 5 to 7 years.

---

**👤 You:**
> "Will my new delivery route be covered under the updated policy?"

**🤖 AI Agent:**
> No, the updated policy now excludes seasonal delivery routes in the northern territory.

---

**👤 You:**
> "Generate a checklist to verify my assets after the policy update."

**🤖 AI Agent:**
> 1. The vehicle [ID-442] meets the new age requirements. (Low Severity)
2. The warehouse [ID-99] satisfies the new geographic bounds. (Low Severity)


## ❓ FAQ

**Q: How does this tool prevent coverage gaps?**
By using `validate_coverage_alignment`, the tool compares your specific asset attributes against the new policy text to identify any mismatches that could lead to a loss of protection.

**Q: Can I map changes to my specific equipment?**
Yes. By providing your list of insured assets to `map_impacts_to_entities`, the tool identifies exactly which items are affected by specific wording changes.

**Q: What is the output of the impact analysis?**
The analysis provides a detailed mapping of policy changes to affected entities and a final confirmation checklist to verify compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/policy-change-impact-brief](https://vinkius.com/en/ai-agent-connect/policy-change-impact-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Policy Change Impact Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `policy-change-impact-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Policy Change Impact Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "policy-change-impact-brief": {
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
