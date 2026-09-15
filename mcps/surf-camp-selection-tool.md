# Surf Camp Selection Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-camp-selection-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Find and rank the perfect surf camps based on your skill, budget, and goals.

## Description
This MCP server acts as an intelligent decision-support engine for surfers. It allows AI agents to evaluate surf camp options by matching user profiles against specific camp characteristics. Using `find_suitable_camps`, agents can filter options by skill level and budget. For more tailored results, `get_recommendation_ranking` provides a prioritized list based on specific objectives like progression or leisure. Users can also use `calculate_value_assessment` to determine if a camp offers good value for money, or `get_camp_details` to retrieve technical specifications like wave consistency and coaching quality.


## Available Tools (4)
- **calculate_value_assessment**: Evaluates the value for money of a specific surf camp
- **find_suitable_camps**: Finds a list of surf camps that match the user's skill level and budget
- **get_camp_details**: Retrieves detailed technical data about a specific surf camp
- **get_recommendation_ranking**: Provides a ranked list of camps based on user profile and goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Camp Selection Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me some beginner surf camps in Portugal within a 1500 Euro budget."

**🤖 AI Agent:**
> I found 3 beginner-friendly camps in Portugal within your 1500 Euro budget: Algarve Surf Base, Sagres Waves, and Peniche Pro.

---

**👤 You:**
> "Which surf camp is best for improving my advanced surfing skills?"

**🤖 AI Agent:**
> Based on your goal of progression, the top-ranked camp is North Shore Pro, which offers high-quality coaching and consistent wave conditions.

---

**👤 You:**
> "Is the Costa Brava Surf Camp a good value for a 2000 Euro budget?"

**🤖 AI Agent:**
> Yes, the Costa Brava Surf Camp offers high value with a score of 8.5/10, as its excellent coaching quality justifies the price.


## ❓ FAQ

**Q: How does the tool determine which camps are suitable?**
The tool uses `find_suitable_camps` to match your skill level and budget against available camp data, ensuring the coaching level meets your proficiency.

**Q: Can I prioritize specific goals like skill progression?**
Yes, by using `get_recommendation_ranking`, the engine weights coaching quality and wave consistency more heavily if your primary goal is progression.

**Q: How is the value of a camp calculated?**
The `calculate_value_assessment` tool compares the camp's total cost against its quality metrics, such as coaching quality and wave consistency, to provide a value score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-camp-selection-tool](https://vinkius.com/en/ai-agent-connect/surf-camp-selection-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Camp Selection Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-camp-selection-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Camp Selection Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-camp-selection-tool": {
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
