# OpenFDA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openfda-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access FDA drug safety data, device recalls, food enforcement reports and approved drug information.

## Description
Connect to **OpenFDA** and explore the FDA's open data platform through natural conversation — no API key needed.

### What you can do

- **Drug Adverse Events** — Search the FDA Adverse Event Reporting System (FAERS) for drug safety reports
- **Device Adverse Events** — Search medical device malfunction and injury reports (MAUDE database)
- **Food Recalls** — Find food product recall enforcement reports with classification and distribution info
- **Drug Labels** — Search structured drug labeling data with ingredients, warnings and dosage info
- **Approved Drugs** — Search Drugs@FDA for approved drug applications with sponsor and approval details
- **Device Recalls** — Find medical device recall enforcement reports
- **Device Clearance** — Search 510(k) premarket device clearance data
- **Animal & Veterinary** — Search adverse event reports for animal drugs and veterinary products

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore FDA safety data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Professionals** — monitor drug safety signals, device malfunctions and recall notifications
- **Researchers** — analyze adverse event patterns, drug safety trends and device performance
- **Patients** — find information about drug side effects, device recalls and food safety alerts


## Available Tools (8)
- **search_animal_events**: Returns reports of adverse events in animals from drug exposure. Use search syntax: animal.species="dog" or drug.active_ingredient="ivermectin".

Search animal and veterinary adverse event reports
- **search_device_clearance**: Returns device names, 510(k) numbers, applicant names, decision dates, regulation numbers and product codes.

Search 510(k) premarket device clearance data
- **search_device_events**: Returns reports of device malfunctions, injuries and deaths. Use search syntax: device.brand_name="pacemaker" or patient.problems.problem_text="infection".

Search medical device adverse event reports
- **search_device_recalls**: Returns recalled devices with reason for recall, classification, recalling firm, product description, code_info and distribution pattern.

Search medical device recall reports
- **search_drugsfda**: Returns drug names, active ingredients, application numbers, sponsors/manufacturers, approval dates and product details. Use search syntax: openfda.brand_name:"Lipitor" or openfda.generic_name:"atorvastatin".

Search FDA-approved drug applications
- **search_drug_events**: Returns adverse events submitted by healthcare professionals, consumers and manufacturers. Use search syntax: patient.reaction.reactionmeddrapt="headache" or openfda.brand_name="Advil". Supports pagination with limit (max 1000) and skip parameters.

Search drug adverse event reports
- **search_drug_labels**: Returns drug labels with active ingredients, purpose, warnings, dosage, indications, manufacturer info and more. Use search syntax: openfda.brand_name:"Advil" or effective_time:"2024".

Search drug labeling information
- **search_food_recalls**: Returns recalled food products with reason for recall, classification (Class I/II/III), recalling firm, distribution and product description.

Search food recall enforcement reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenFDA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me recent adverse events for Advil."

**🤖 AI Agent:**
> Found 10 recent adverse event reports for Advil (ibuprofen). Common reactions: nausea (142 reports), headache (98 reports), dizziness (76 reports), abdominal pain (54 reports). Reports submitted by healthcare professionals and consumers between 2023-2024.

---

**👤 You:**
> "What food recalls are currently active?"

**🤖 AI Agent:**
> Found 5 active food recalls: 1. Listeria in deli meats (Class I, high risk) — 2. Salmonella in peanut butter (Class I) — 3. Undeclared allergen in snack bars (Class II) — 4. Metal fragments in frozen meals (Class I) — 5. Mold contamination in juice (Class II).

---

**👤 You:**
> "Find FDA-approved drugs containing atorvastatin."

**🤖 AI Agent:**
> Found 15 FDA-approved drug applications containing atorvastatin. Notable: Lipitor (Pfizer, approved 1996), Atorvastatin Calcium (generic, multiple sponsors), Liptruzet (Merck). Includes application numbers, approval dates, dosage forms and strengths.


## ❓ FAQ

**Q: Do I need an API key?**
No! OpenFDA data is completely free and open. No authentication required. Just subscribe and start searching. Rate limit is 240 requests/minute for unauthenticated access.

**Q: What search syntax should I use?**
Use Lucene query syntax: openfda.brand_name:"Advil" for brand names, patient.reaction.reactionmeddrapt:"headache" for reactions, event_type:"Injury" for device events. Combine with AND/OR operators.

**Q: What are drug adverse events?**
Drug adverse events are safety reports submitted to the FDA about potential side effects from medications. Reports come from healthcare professionals, consumers and manufacturers. They do NOT prove the drug caused the event — just that the event was reported while the patient was taking the drug.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfda-alternative](https://vinkius.com/mcp/openfda-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenFDA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openfda-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenFDA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openfda-alternative": {
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
