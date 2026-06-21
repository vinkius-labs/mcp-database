# Cloud Assess MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloud-assess)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage vocational training and assessments via Cloud Assess — track students, monitor enrolments, and audit assessment records directly from any AI agent.

## Description
Connect your **Cloud Assess** account to any AI agent and take full control of your RTO (Registered Training Organisation) operations through natural conversation. Streamline how you manage student progress and assessment compliance natively.

### What you can do

- **Student Oversight** — List and retrieve details for all students (members) in your system natively
- **Enrolment Intelligence** — Access and monitor student enrolments in qualifications and individual units flawlessly
- **Assessment Management** — List and review assessment results, outcomes, and evidence records securely
- **Unit Progress Tracking** — Monitor progress and completion status at the unit enrolment level flawlessly
- **Form & Checklist Auditing** — Access specific assessment forms and data points directly within your workspace flawlessly
- **Staff Visibility** — List internal trainers and assessors who manage the training delivery flawlessly

### How it works

1. Subscribe to this server
2. Enter your Cloud Assess Client Key and API Key
3. Start managing your training data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Training Managers** — monitor student completion rates and compliance using natural language
- **Assessors** — review individual assessment records and evidence without opening the core application
- **RTO Administrators** — quickly look up student enrolments and training locations straight from their chat interface
- **Compliance Officers** — verify assessment outcomes and form records for audit preparation


## Available Tools (8)
- **get_student_details**: Get detailed information for a specific student
- **list_assessment_records**: List individual assessment results and evidence records
- **list_training_assessors**: List all internal assessors and trainers
- **list_training_enrolments**: List student enrolments in qualifications or units
- **list_assessment_forms**: List specific forms and checklists captured within assessments
- **list_training_locations**: List physical or logical training locations
- **list_student_members**: List all students (members) in Cloud Assess
- **list_unit_enrolment_progress**: List progress and status at the unit enrolment level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloud Assess** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all students currently enrolled in the 'Diploma of Management'."

**🤖 AI Agent:**
> Retrieving enrolments for 'Diploma of Management'... I found 12 students currently enrolled. The list includes John Doe, Sarah Smith, and 10 others. Would you like to see their individual progress?

---

**👤 You:**
> "Show me the assessment results for student ID 'STU_12345'."

**🤖 AI Agent:**
> Checking assessment records for STU_12345... This student has 5 completed assessments. 4 are marked as 'Satisfactory' and 1 is 'Pending Review' by an assessor.

---

**👤 You:**
> "Who is the assessor assigned to the 'Unit BSB401' for John Doe?"

**🤖 AI Agent:**
> Retrieving unit enrolment details... The assigned assessor for John Doe's BSB401 unit is Mike Scott. I can provide his contact info if you need to follow up.


## ❓ FAQ

**Q: Can I see if a student has completed a specific unit?**
Yes! Use the `list_unit_enrolment_progress` tool. The agent will return the progress status and current outcome for students across their enrolled units.

**Q: How do I check the latest assessment evidence uploaded for a student?**
Use the `list_assessment_records` tool. Your agent will fetch individual assessment entries, which include metadata about the evidence provided and the final outcome.

**Q: Where do I find my Cloud Assess API keys?**
You can find your **Client Key** and **API Key** in your Cloud Assess account under the integration or developer settings. You may need administrator access to view these.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloud-assess](https://vinkius.com/mcp/cloud-assess)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloud Assess** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloud-assess` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloud Assess** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloud-assess": {
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
