# Gym Buddy Matching Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gym-buddy-matching-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate gym partner compatibility and find optimal training windows.

## Description
This MCP server helps users find the perfect workout partner by analyzing training profiles. Use `calculate_compatibility` to determine how well two users align on goals and style, or `find_optimal_training_windows` to identify shared availability. You can also use `analyze_training_synergy` to understand how partners can support each other's fitness journey, or `get_matching_tiers` to see different partnership levels like Elite Pairings or Steady Partners.


## Available Tools (4)
- **find_optimal_training_windows**: Identifies specific days and times when two users can meet
- **analyze_training_synergy**: Provides a qualitative description of how the users can help each other
- **calculate_compatibility**: Determines the overall fitness of a potential partnership
- **get_matching_tiers**: Filters potential matches based on the degree of similarity required


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gym Buddy Matching Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the compatibility between User A (Goal: Muscle Gain, Style: Heavy Lifting, Experience: Advanced) and User B (Goal: Muscle Gain, Style: Heavy Lifting, Experience: Intermediate)."

**🤖 AI Agent:**
> The compatibility score is 85. The users have highly aligned goals and styles, making them strong partners for heavy lifting sessions.

---

**👤 You:**
> "Find the best training times for two users with these schedules: User A ['Mon 10:00-12:00', 'Wed 14:00-16:00'] and User B ['Mon 11:00-13:00', 'Fri 09:00-11:00']."

**🤖 AI Agent:**
> The optimal training window is Monday from 11:00 to 12:00.

---

**👤 You:**
> "What are the different matching tiers available?"

**🤖 AI Agent:**
> Available tiers include Elite Pairings for identical goals, Steady Partners for aligned goals, and Exploratory Partners for cross-training.


## ❓ FAQ

**Q: How do I calculate if two people are a good match?**
You can use the `calculate_compatibility` tool by providing the training profiles for both users.

**Q: Can I find out when my gym partner is available?**
Yes, use the `find_optimal_training_windows` tool with both users' weekly schedules to find overlapping times.

**Q: What kind of synergy analysis can I get?**
The `analyze_training_synergy` tool provides a qualitative description of how users can help each other, such as Mentorship or High Alignment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gym-buddy-matching-score](https://vinkius.com/en/ai-agent-connect/gym-buddy-matching-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gym Buddy Matching Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gym-buddy-matching-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gym Buddy Matching Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gym-buddy-matching-score": {
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
