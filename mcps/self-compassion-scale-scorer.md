# Self-Compassion Scale Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/self-compassion-scale-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate psychological self-compassion profiles and receive actionable wellness insights.

## Description
This MCP server provides a specialized engine to calculate psychological scores based on the Self-Compassion Scale (SCS). It processes raw survey responses to determine a user's total self-compassion score and detailed subdomain metrics including self-kindness, common humanity, and mindfulness. Users can also retrieve specific guidance for deficits like self-judgment, isolation, or over-identification. Use `score_scs_responses` to generate a full profile or `get_subdomain_insights` for targeted recommendations.


## Available Tools (4)
- **get_scale_metadata**: Retrieve the structural definition of the scale (item lists and types)
- **score_scs_responses**: Calculate the comprehensive self-compassion profile from a set of raw survey responses
- **get_subdomain_insights**: Provide specific, actionable psychological guidance based on a particular subdomain score
- **validate_response_set**: Ensure a set of raw data is structurally sound and complete before attempting heavy computation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Self-Compassion Scale Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you score these SCS responses for me? {"item1": 4, "item2": 3, "item3": 5}"

**🤖 AI Agent:**
> Your total self-compassion score is 4.0. Your profile shows high levels of self-kindness and mindfulness.

---

**👤 You:**
> "I scored a 2 on the self-judgment subdomain. What should I do?"

**🤖 AI Agent:**
> To address self-judgment, try practicing self-kindness by speaking to yourself as you would to a dear friend during difficult moments.

---

**👤 You:**
> "What are the subdomains measured by the Self-Compassion Scale?"

**🤖 AI Agent:**
> The scale measures self-kindness, common humanity, and mindfulness, while also identifying deficits in self-judgment, isolation, and over-identification.


## ❓ FAQ

**Q: How do I prepare my data for scoring?**
You should first use `validate_response_set` to ensure your JSON object of item identifiers and numerical values is complete and structurally sound.

**Q: Can I get specific advice for my results?**
Yes, after calculating your profile with `score_scs_responses`, you can use `get_subdomain_insights` to receive qualitative suggestions for practice or reflection.

**Q: What tools are available in this MCP?**
The server includes `score_scs_responses` for full profiling, `get_subdomain_insights` for guidance, `validate_response_set` for data integrity, and `get_scale_metadata` for scale structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/self-compassion-scale-scorer](https://vinkius.com/en/ai-agent-connect/self-compassion-scale-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Self-Compassion Scale Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `self-compassion-scale-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Self-Compassion Scale Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "self-compassion-scale-scorer": {
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
