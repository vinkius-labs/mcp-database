# Local Experience Feedback Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-feedback-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured, factual, and low-disclosure feedback plans for local experiences.

## Description
This MCP server provides a systematic engine for transforming raw observations of local experiences into constructive feedback. By adhering to the Facts-Only Principle and Minimum-Disclosure rules, it ensures that feedback is professional, objective, and respects user privacy. Use `analyze_experience_observations` to transform raw data into a structured plan, `verify_evidence_validity` to ensure claims are supported by facts, `determine_submission_strategy` to find the best delivery method, and `evaluate_participation_outlook` to decide on future engagement.


## Available Tools (4)
- **analyze_experience_observations**: Process raw experience data into structured factual observations and a constructive message
- **determine_submission_strategy**: Identify the best way to deliver the feedback based on organizer channel and booking facts
- **evaluate_participation_outlook**: Decide if the user should participate in similar experiences in the future
- **verify_evidence_validity**: Validate that the collected observations are sufficient to support the requested feedback


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Feedback Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I went to a cafe. The coffee was cold and it took 25 minutes to arrive, even though I was promised 5 minutes. I wanted a quick breakfast. I don't want them to have my email."

**🤖 AI Agent:**
> Constructive Message: The coffee was served at a low temperature, and the wait time was 25 minutes despite a 5-minute expectation. 
Evidence Checklist: [Coffee temperature, 25-minute wait time, 5-minute promise] 
Submission Action: Use the cafe's digital feedback portal. 
Response-Review Plan: Monitor the portal for a response within 3 business days. 
Future Participation: Caution.

---

**👤 You:**
> "The guided tour was great, but the guide arrived 15 minutes late. I wanted a punctual start. I am happy to share my booking details."

**🤖 AI Agent:**
> Constructive Message: The tour guide arrived 15 minutes after the scheduled start time. 
Evidence Checklist: [15-minute delay] 
Submission Action: Contact the organizer via their official email. 
Response-Review Plan: Check for an email acknowledgment within 48 hours. 
Future Participation: Proceed.

---

**👤 You:**
> "The hotel room was not cleaned by 3 PM as promised. I wanted a clean room upon arrival. I am very upset and don't want to talk to them."

**🤖 AI Agent:**
> Constructive Message: The room was not cleaned by the promised time of 3 PM. 
Evidence Checklist: [Room not cleaned by 3 PM] 
Submission Action: Submit an anonymous message through the booking platform. 
Response-Review Plan: Review the platform's resolution status. 
Future Participation: Avoid.


## ❓ FAQ

**Q: How does this tool ensure my privacy?**
The system applies Minimum-Disclosure rules and cross-references all observations against your specified `privacyBoundaries` to ensure no sensitive data is included in the final feedback.

**Q: What is the 'Facts-Only Principle'?**
It is a core rule that ensures feedback is derived only from observable events rather than emotional judgments, making the feedback more professional and effective.

**Q: Can I use this for high-end services?**
Yes. The engine uses EXPERIENCE_TIERS to adjust the depth of evidence required and the strictness of privacy rules based on whether the experience is Casual, Standard, or Premium.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-feedback-planner](https://vinkius.com/en/ai-agent-connect/local-experience-feedback-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Feedback Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-feedback-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Feedback Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-feedback-planner": {
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
