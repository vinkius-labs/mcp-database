# Life Satisfaction Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/life-satisfaction-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify and reflect on life satisfaction using the validated SWLS scale.

## Description
This MCP server provides a specialized toolkit for evaluating psychological life satisfaction. It implements the validated Satisfaction with Life Scale (SWLS) to transform raw survey responses into meaningful insights. Users can use `validate_response_format` to check their inputs, `calculate_swls_score` to determine their satisfaction category, `compare_to_norms` to see how they rank against population distributions, and `get_reflection_prompts` to receive personalized qualitative questions for deeper self-exploration.


## Available Tools (4)
- **calculate_swls_score**: Calculates the raw total score and the qualitative satisfaction category for a given set of responses
- **compare_to_norms**: Compares a specific total score against established population distribution norms
- **get_reflection_prompts**: Generates personalized qualitative questions to help the user reflect on their life satisfaction
- **validate_response_format**: Ensures a user's input data adheres to the requirements of the SWLS instrument before calculation begins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Life Satisfaction Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I answered 7, 6, 7, 7, 6 on the life satisfaction scale. What is my score and category?"

**🤖 AI Agent:**
> Your total score is 33, which falls into the High Satisfaction category.

---

**👤 You:**
> "My score was 12. How does this compare to the general population?"

**🤖 AI Agent:**
> A score of 12 is in the low percentile compared to the general population.

---

**👤 You:**
> "I got a score of 25. Can you give me some reflection prompts?"

**🤖 AI Agent:**
> Since you have moderate satisfaction, consider reflecting on which areas of your life are currently providing the most stability.


## ❓ FAQ

**Q: What is the SWLS?**
The Satisfaction with Life Scale (SWLS) is a validated psychometric instrument used to measure cognitive judgments of life satisfaction.

**Q: How do I format my responses?**
You should provide an array of exactly five integers, where each integer is between 1 and 7, representing your answers to the scale items.

**Q: Can I compare my score to others?**
Yes, you can use the `compare_to_norms` tool to see your percentile relative to established population distributions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/life-satisfaction-scorer](https://vinkius.com/en/ai-agent-connect/life-satisfaction-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Life Satisfaction Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `life-satisfaction-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Life Satisfaction Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "life-satisfaction-scorer": {
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
