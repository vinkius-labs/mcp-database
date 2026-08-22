# Roommate Compatibility Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/roommate-compatibility-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate deterministic roommate compatibility and fair rent splits for Singapore living.

## Description
This MCP server provides a deterministic engine to evaluate living arrangements for young adults in Singapore. It calculates a compatibility score based on lifestyle pillars like cleanliness, noise tolerance, guest policies, and cooking frequency. It also identifies critical deal breakers such as smoking habits or pet allergies. Additionally, it helps determine a fair rent split based on the physical size of bedrooms in HDB or condo settings. Use `calculate_compatibility_score` to find your match quality, `calculate_rent_split` for financial fairness, and `get_compatibility_summary` for a quick decision-making overview.


## Available Tools (3)
- **get_compatibility_summary**: Provides a high-level overview of the match status for quick decision-making
- **calculate_compatibility_score**: Evaluates the total compatibility between two individuals based on their lifestyle preferences and deal breakers
- **calculate_rent_split**: Determines a fair distribution of monthly rent based on the physical dimensions of the bedrooms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roommate Compatibility Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the compatibility score for two roommates. Person A: clean_schedule='Daily', noise_tolerance='Low', guest_policy='Weekends Only', cooking_frequency='Frequently', smokes=false, has_pets=false. Person B: clean_schedule='Daily', noise_tolerance='Low', guest_policy='Weekends Only', cooking_frequency='Frequently', smokes=true, has_pets=false."

**🤖 AI Agent:**
> { "compatibilityScore": 0, "dealBreakersDetected": ["smoking"], "compatibilityTier": "Avoid" }

---

**👤 You:**
> "How should we split a $1500 rent if my room is 12sqm and my roommate's room is 18sqm?"

**🤖 AI Agent:**
> { "myShare": 600, "roommateShare": 900 }

---

**👤 You:**
> "Is a match with a score of 85 and no deal breakers viable?"

**🤖 AI Agent:**
> { "isViable": true, "recommendationMessage": "This is a Good match. You are highly compatible!" }


## ❓ FAQ

**Q: How is the compatibility score calculated?**
The score is calculated by matching four lifestyle pillars: cleanliness, noise, guests, and cooking. Each match adds 25 points. If deal breakers like smoking or pet allergies are detected, the score is reduced by 100.

**Q: How does the rent split tool work?**
The `calculate_rent_split` tool distributes the total rent proportionally based on the square meterage of each individual's room.

**Q: What are deal breakers?**
Deal breakers are non-negotiable conflicts, such as one person smoking while the other does not, or pet-related allergies, which significantly impact the compatibility score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/roommate-compatibility-score](https://vinkius.com/ai-agent-connect/roommate-compatibility-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roommate Compatibility Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roommate-compatibility-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roommate Compatibility Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roommate-compatibility-score": {
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
