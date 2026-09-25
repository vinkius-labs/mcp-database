# Photography Subject Consent Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photography-subject-consent-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal-compliance](../categories/legal-compliance.md)

A specialized planning engine for photographers to manage legal consent, usage rights, and privacy workflows.

## Description
This MCP server provides a comprehensive workflow for photographers to secure, document, and manage legal consent from human subjects. It ensures all image usage strictly adheres to agreed-upon privacy and release terms. Photographers can use `contact_subject` to initiate professional outreach, `generate_consent_agenda` to prepare for live discussions, and `create_usage_record` to formalize legal agreements. The engine also includes `design_delivery_plan` for asset transfer and `manage_consent_exception` to handle unexpected events like consent withdrawal.


## Available Tools (5)
- **contact_subject**: Generates a professional communication to initiate the consent process
- **create_usage_record**: Formalizes the agreed-upon usage rights into a structured record
- **design_delivery_plan**: Outlines how the final images will be transferred to the subject or stakeholders
- **generate_consent_agenda**: Creates a structured talking points list for a live discussion
- **manage_consent_exception**: Provides a workflow for handling unexpected events like consent withdrawal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photography Subject Consent Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to reach out to Jane Doe for a street photography session in downtown London. How should I start?"

**🤖 AI Agent:**
> Subject: Photography Session Inquiry - Downtown London. Dear Jane Doe, I am planning a photography session in the downtown London area and would love to include you in the shoot. The images are intended for social media and personal archives. I will follow up shortly to discuss consent details.

---

**👤 You:**
> "Create a discussion agenda for a subject named Mark regarding a commercial shoot with perpetual usage rights."

**🤖 AI Agent:**
> Discussion Points: 1. Purpose of the commercial shoot. 2. Scope of perpetual usage rights. 3. Geographic limitations. Key Questions: Will you require credit in all media? Are there specific platforms you wish to exclude?

---

**👤 You:**
> "A subject has withdrawn consent for images that are already published online. What should I do?"

**🤖 AI Agent:**
> Immediate Actions: 1. Remove the images from all online platforms immediately. 2. Notify any third-party distributors. 3. Document the removal in your usage logs.


## ❓ FAQ

**Q: How does this help with legal compliance?**
By using `create_usage_record`, you generate a structured record of the agreed-upon usage rights, ensuring you have a clear paper trail of the subject's permission.

**Q: Can I handle a subject withdrawing their consent?**
Yes, the `manage_consent_exception` tool provides a specific workflow for handling consent revocation and mitigation steps.

**Q: What happens if a subject has specific privacy needs?**
You can use `design_delivery_plan` to ensure that privacy requests, such as blurring or anonymization, are executed before assets are delivered.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photography-subject-consent-plan](https://vinkius.com/en/ai-agent-connect/photography-subject-consent-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photography Subject Consent Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photography-subject-consent-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photography Subject Consent Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photography-subject-consent-plan": {
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
