# Video Participant Release Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/video-participant-release-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media-management](../categories/media-management.md)

Manage participant consent, outreach, and usage rights for video productions.

## Description
This MCP server provides a complete framework for managing the lifecycle of video participant consent. It connects AI agents to specialized tools for generating outreach schedules via `get_outreach_plan`, creating verbal talking points with `generate_discussion_prompts`, and formalizing agreements through `create_consent_record`. It also handles compliance by providing `get_withdrawal_protocol` for revoking consent and `validate_use_change_request` to ensure new video uses stay within legal boundaries.


## Available Tools (5)
- **create_consent_record**: Constructs the formal data structure representing the signed agreement
- **generate_discussion_prompts**: Creates specific talking points to ensure participants understand their rights
- **get_outreach_plan**: Generates a step-by-step communication schedule to secure participation
- **get_withdrawal_protocol**: Provides the immediate action plan when a participant requests to revoke consent
- **validate_use_change_request**: Determines if a proposed change in video usage is permitted under existing consent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Video Participant Release Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create an outreach plan for a minor named Alex for an educational video on YouTube."

**🤖 AI Agent:**
> The outreach plan for Alex includes: 1. Contacting the legal guardian to present the educational purpose. 2. Sending the formal release terms to the guardian. 3. Once signed, notifying Alex of the agreement.

---

**👤 You:**
> "I need talking points to explain the release terms for a commercial video on TV."

**🤖 AI Agent:**
> The discussion prompts are: 'Do you understand that this footage will be broadcast on television?' and 'Are you aware that the usage is limited to commercial advertising as specified in the terms?'

---

**👤 You:**
> "Check if we can move our video from a private website to Instagram."

**🤖 AI Agent:**
> The request requires new consent because Instagram is not included in the original distribution channels specified in the current consent record.


## ❓ FAQ

**Q: How do I handle a minor's consent?**
Use `get_outreach_plan` to generate a sequence that prioritizes contacting the authorized guardian or legal representative before the participant.

**Q: Can I use a video on a new platform after consent is signed?**
You must first use `validate_use_change_request` to check if the new distribution channel is covered by the existing agreement. If not, new consent is required.

**Q: What happens if a participant wants to withdraw?**
Call `get_withdrawal_protocol` to receive specific instructions for handling the request, which will distinguish between stopping future use and removing existing footage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/video-participant-release-manager](https://vinkius.com/en/ai-agent-connect/video-participant-release-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Video Participant Release Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `video-participant-release-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Video Participant Release Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "video-participant-release-manager": {
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
