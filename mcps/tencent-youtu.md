# Tencent Youtu / 腾讯优图 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-youtu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading computer vision platform — perform facial recognition, analysis, and liveness checks via AI.

## Description
Empower your AI agent to orchestrate your visual intelligence and facial recognition workflows with **Tencent Youtu** (腾讯优图), the premier computer vision platform in China. By connecting Youtu to your agent, you transform complex image analysis, face comparison, and person management into a natural conversation. Your agent can instantly detect faces in image URLs, retrieve detailed attributes like age and beauty scores, compare identities across different photos, and manage secure person libraries without you ever needing to navigate the comprehensive Tencent Cloud Console. Whether you are building an automated KYC system or conducting a digital asset audit for facial content, your agent acts as a real-time computer vision specialist, providing accurate and fast results from a single, authorized source.

### What you can do

- **Facial Orchestration** — Detect faces, analyze attributes (gender, age, beauty), and perform static liveness checks.
- **Identity Comparison** — Calculate similarity scores between two face images to verify identities with high precision.
- **Library Management** — Register new persons, list group members, and manage unique identity identifiers.
- **Face Discovery** — Search for matching faces within specific person groups to automate recognition workflows.
- **System Monitoring** — Verify API connectivity and monitor service status to ensure visual intelligence reliability.

### How it works

1. Subscribe to this server
2. Enter your Tencent Cloud SecretId and SecretKey
3. Start managing your visual intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security & Compliance Teams** — automate identity verification and monitor visual access logs through natural language queries.
- **App Developers** — integrate world-class facial recognition and analysis capabilities into your AI-driven daily routines.
- **Content Moderators** — audit visual assets for facial content and metadata directly from your AI-powered workspace.
- **Tencent Cloud Power Users** — integrate your existing IAI/Youtu workflows into your AI-driven daily routines.


## Available Tools (8)
- **list_persons_in_group**: List persons in group
- **live_face_check**: Detect live face
- **register_person**: Create a new person
- **search_face_in_groups**: Search face in library
- **analyze_face**: Analyze facial attributes
- **compare_faces**: Compare two faces
- **detect_face**: Detect faces in image
- **list_face_groups**: List person groups


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent Youtu / 腾讯优图** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Detect faces in this image: [URL] and show me their attributes."

**🤖 AI Agent:**
> I've analyzed the image. I detected one face belonging to a male, approximately 28 years old, with a beauty score of 82/100. Should I search for this person in your registered groups?

---

**👤 You:**
> "Compare these two face images: [URL_A] and [URL_B]."

**🤖 AI Agent:**
> The facial comparison is complete. The similarity score is 94.5, indicating a very high probability that these are the same person. Would you like me to check if this identity is already registered in your person library?

---

**👤 You:**
> "Register a new person 'Alice' in group 'staff_01' with image [URL]."

**🤖 AI Agent:**
> Alice has been successfully registered in group `staff_01` with ID `alice_8821`. Her facial features have been indexed for future recognition. Should I list all members currently in this group?


## ❓ FAQ

**Q: How do I find my Tencent Cloud SecretId and SecretKey?**
Log in to the [Tencent Cloud Console](https://console.cloud.tencent.com/), navigate to [Access Management] -> [API Key Management] to find or generate your unique SecretId and SecretKey.

**Q: What is the 'Beauty' score?**
The Beauty score is an aesthetic metric provided by the Tencent Youtu AI, ranging from 0 to 100. It is a technical attribute intended for entertainment and lifestyle application scenarios.

**Q: Does this server handle signature calculation?**
Yes! The server automatically calculates the required TC3-HMAC-SHA256 signature for every request using your provided SecretKey, ensuring secure authorized communication with the Tencent Cloud AI gateway.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-youtu](https://vinkius.com/mcp/tencent-youtu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent Youtu / 腾讯优图** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tencent-youtu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent Youtu / 腾讯优图** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-youtu": {
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
