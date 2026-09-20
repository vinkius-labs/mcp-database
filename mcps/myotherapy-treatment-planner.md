# Myotherapy Treatment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/myotherapy-treatment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Generates clinical myotherapy treatment plans based on pain, trigger points, and movement restrictions.

## Description
This MCP server provides specialized clinical logic to assist practitioners in designing effective myotherapy sessions. By analyzing clinical presentations including pain locations, trigger points, and muscle dysfunction, the engine uses `get_treatment_plan` to generate structured treatment areas, specific technique selections, and time allocations. It also includes tools like `get_technique_details` for clinical information, `validate_home_care` to ensure exercise safety, and `calculate_session_efficiency` to verify that treatment density is realistic for clinical practice.


## Available Tools (4)
- **calculate_session_efficiency**: Evaluates the density of the treatment plan to ensure it is realistic for a standard clinical appointment
- **get_technique_details**: Provides detailed clinical information regarding a specific myotherapy technique
- **get_treatment_plan**: Generates a comprehensive clinical treatment plan based on a patient's specific physical symptoms
- **validate_home_care**: Checks if a proposed set of home exercises is appropriate for the reported movement restrictions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Myotherapy Treatment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a treatment plan for a patient with lower back pain, a trigger point in the quadratus lumborum, and limited lumbar flexion."

**🤖 AI Agent:**
> The treatment plan includes addressing the lumbar region with ischemic compression for the trigger point and myofascial release for the surrounding muscle tension, totaling 45 minutes.

---

**👤 You:**
> "What are the details for the 'Ischemic Compression' technique?"

**🤖 AI Agent:**
> Ischemic Compression is a manual therapy technique used to treat trigger points by applying sustained pressure to the hyperirritable spot to improve local blood flow.

---

**👤 You:**
> "Is it safe to recommend 'Cat-Cow' stretches for a patient with acute lumbar disc irritation?"

**🤖 AI Agent:**
> The exercise is considered unsafe for this specific restriction as the spinal flexion might exacerbate the disc irritation.


## ❓ FAQ

**Q: How does the tool generate a treatment plan?**
The `get_treatment_plan` tool processes the reported pain locations, trigger points, and muscle dysfunctions to map them against standardized myotherapy protocols.

**Q: Can I check if exercises are safe for my patient?**
Yes, you can use `validate_home_care` to check if a specific list of exercises is appropriate given the patient's reported movement restrictions.

**Q: How do I know if my planned session is too long or too short?**
The `calculate_session_efficiency` tool evaluates the planned duration against the number of treatment areas to ensure the session is clinically feasible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/myotherapy-treatment-planner](https://vinkius.com/en/ai-agent-connect/myotherapy-treatment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Myotherapy Treatment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `myotherapy-treatment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Myotherapy Treatment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "myotherapy-treatment-planner": {
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
