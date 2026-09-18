# Cognitive Reserve Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cognitive-reserve-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Estimate cognitive reserve and get brain health insights.

## Description
This MCP server provides tools to estimate an individual's cognitive reserve--the brain's resilience against decline. Users can use `estimate_cognitive_reserve` to calculate a reserve score based on education, occupation, and lifestyle. It also includes `get_health_recommendations` for actionable lifestyle changes, `analyze_occupational_impact` to evaluate professional mental demand, and `evaluate_social_and_cognitive_activity` to assess current mental and social engagement.


## Available Tools (4)
- **analyze_occupational_impact**: Evaluates how much a user's current or past work contributes to their cognitive buffer
- **estimate_cognitive_reserve**: Calculates the primary cognitive reserve score and identifies key protective drivers
- **evaluate_social_and_cognitive_activity**: Analyzes the "active reserve" being maintained through current lifestyle choices
- **get_health_recommendations**: Provides personalized lifestyle adjustments based on a calculated reserve


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cognitive Reserve Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate my cognitive reserve. I have 16 years of education, my job is High complexity, I am bilingual, and my stimulation and social levels are both 7."

**🤖 AI Agent:**
> Your cognitive reserve score is 78, which is considered High. Your primary drivers are bilingualism and high occupational complexity.

---

**👤 You:**
> "What are some ways I can improve my brain health based on a score of 45?"

**🤖 AI Agent:**
> To improve your score, focus on increasing social engagement and finding more cognitively stimulating hobbies like learning a new language.

---

**👤 You:**
> "How much has my 10 years in a High complexity role contributed to my reserve?"

**🤖 AI Agent:**
> Your total occupational contribution is 45, consisting of a 35 point complexity impact and a 10 point longevity bonus.


## ❓ FAQ

**Q: What is cognitive reserve?**
Cognitive reserve is the brain's ability to improvise and find alternate ways of getting a job done, providing resilience against neurodegeneration.

**Q: How can I improve my score?**
You can use `get_health_recommendations` to receive personalized suggestions for increasing your cognitive and social engagement.

**Q: Does my job affect my cognitive reserve?**
Yes, you can use `analyze_occupational_impact` to see how the complexity and duration of your professional roles contribute to your cognitive buffer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cognitive-reserve-estimator](https://vinkius.com/en/ai-agent-connect/cognitive-reserve-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cognitive Reserve Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cognitive-reserve-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cognitive Reserve Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cognitive-reserve-estimator": {
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
