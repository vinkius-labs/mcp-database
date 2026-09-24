# Pet Medical Record Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-medical-record-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Audit and summarize medical record volumes for specific pets.

## Description
This MCP server provides tools to audit and summarize the volume of medical history entries for animal patients. Use `get_pet_record_count` to find the exact number of clinical entries and visits for a specific pet, or `get_pet_history_summary` to check if a pet's clinical file is complete based on their activity level. You can also use `list_pets_by_record_threshold` to identify pets with specific record counts or `validate_file_integrity` to ensure data files are structurally sound.


## Available Tools (4)
- **get_pet_history_summary**: Answers what the high-level clinical status and activity level of this pet is
- **get_pet_record_count**: Answers how many individual medical records exist for this specific pet
- **list_pets_by_record_threshold**: Answers which pets in the database have an unusually high or low number of medical records
- **validate_file_integrity**: Answers if the provided pet data file is structurally sound and containing valid identifiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Medical Record Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many medical records does pet ID 12345 have?"

**🤖 AI Agent:**
> Pet ID 12345 has 12 individual medical records and 4 distinct clinical visits.

---

**👤 You:**
> "Give me a summary of the clinical status for pet 98765."

**🤖 AI Agent:**
> Pet 98765 has a complete clinical history with 8 total records. The last visit was on 2023-11-15.

---

**👤 You:**
> "Which pets have at least 10 medical records?"

**🤖 AI Agent:**
> The following pets meet the threshold: Pet ID 111 (12 records), Pet ID 222 (15 records), and Pet ID 333 (10 records).


## ❓ FAQ

**Q: How can I check if a pet's medical history is complete?**
You can use the `get_pet_history_summary` tool, which returns an `isComplete` status indicating if the pet has sufficient history for clinical decisions.

**Q: How do I find pets with a high number of medical records?**
Use the `list_pets_by_record_threshold` tool and set the `minRecords` parameter to your desired minimum threshold.

**Q: Can I verify the integrity of a data file?**
Yes, the `validate_file_integrity` tool allows you to check if a pet data file is structurally sound and contains valid identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-medical-record-auditor](https://vinkius.com/en/ai-agent-connect/pet-medical-record-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Medical Record Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-medical-record-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Medical Record Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-medical-record-auditor": {
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
