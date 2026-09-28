# Local Experience Post-Visit Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-post-visit-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [personalization](../categories/personalization.md)

Processes participant feedback and provider constraints to manage privacy, engagement, and future visits.

## Description
This MCP server acts as a post-visit intelligence engine. It reconciles user sentiment with provider policies to automate critical post-experience workflows. Using `analyze_privacy_and_sharing`, it determines data visibility based on consent. It uses `generate_engagement_actions` to draft thank-you notes or issue reports, and `evaluate_return_viability` to check if return visits are permitted under provider terms. Additionally, it can `synthesize_user_records` to preserve important memories and `construct_next_experience_prompt` to suggest future activities based on previous impressions.


## Available Tools (5)
- **analyze_privacy_and_sharing**: Determines if the experience data can be made public or shared with others based on user consent and provider terms
- **synthesize_user_records**: Identifies which parts of the experience the user wants to preserve in their history
- **construct_next_experience_prompt**: Generates a personalized suggestion for the user's next activity
- **evaluate_return_viability**: Analyzes if the user should return based on the experience outcome and provider policies
- **generate_engagement_actions**: Determines the appropriate thank-you or feedback responses to send to the provider


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Post-Visit Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I had a great time at the pottery workshop, but I'm not sure if I can share the photos I took."

**🤖 AI Agent:**
> Based on your feedback, your data can be kept private. Since you enjoyed the workshop, I can also help you draft a thank-you note to the instructor.

---

**👤 You:**
> "The guided tour was okay, but the guide was late and it was quite frustrating."

**🤖 AI Agent:**
> I have flagged this as a high priority issue. I will draft a formal feedback report regarding the guide's tardiness to help resolve this with the provider.

---

**👤 You:**
> "I loved the mountain biking trip! I want to do more outdoor adventures next month."

**🤖 AI Agent:**
> Since you enjoyed the mountain biking, how about exploring some local trail running routes or a forest hiking excursion next month?


## ❓ FAQ

**Q: How does the server handle user privacy?**
The `analyze_privacy_and_sharing` tool ensures that data is only shared if explicit user consent is provided and no provider terms prohibit it.

**Q: Can I automate thank-you notes to providers?**
Yes, `generate_engagement_actions` creates appropriate responses, such as thank-you notes for positive experiences or issue reports for unresolved problems.

**Q: How are future activity suggestions generated?**
The `construct_next_experience_prompt` tool uses both the user's future interests and their previous impressions to create personalized suggestions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-post-visit-plan](https://vinkius.com/en/ai-agent-connect/local-experience-post-visit-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Post-Visit Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-post-visit-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Post-Visit Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-post-visit-plan": {
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
