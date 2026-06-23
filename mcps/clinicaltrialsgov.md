# ClinicalTrials.gov MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clinicaltrialsgov)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search the world's largest registry of clinical research studies — covering diseases, drugs, and experimental therapies across all phases.

## Description
The **ClinicalTrials.gov MCP Server** connects your AI agent to the United States National Institutes of Health (NIH) clinical research database — the gold standard for clinical trial transparency worldwide.

### Core Capabilities

- **Universal Trial Search** — Query over 500,000 registered studies by condition, drug name, sponsor, or any keyword. Filter by recruitment status and trial phase to pinpoint exactly what matters.
- **Deep Trial Profiles** — Retrieve full study protocols including eligibility criteria, enrollment targets, intervention details, and sponsor information for any registered trial.
- **Active Recruitment Finder** — Dedicated tool for patients and clinicians to discover trials actively enrolling participants right now, searchable by medical condition.

Zero authentication required. Fully open public data maintained by the National Library of Medicine. Critical for pharmaceutical researchers, healthcare professionals, patient advocates, and biotech analysts.


## Available Tools (3)
- **find_recruiting_trials**: Useful for patients and healthcare providers looking for active enrollment opportunities.

Find clinical trials that are actively recruiting participants for a specific medical condition
- **get_trial_details**: Retrieve full details of a specific clinical trial by its NCT identifier
- **search_clinical_trials**: Can filter by recruitment status and trial phase.

Search the ClinicalTrials.gov database for studies by keyword, condition, drug name, or sponsor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClinicalTrials.gov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any clinical trials recruiting participants for Alzheimer's disease right now?"

**🤖 AI Agent:**
> I found several actively recruiting Alzheimer's trials. For example, NCT07011745 is a Phase 3 randomized trial with 352 targeted participants, testing a new therapeutic approach. There are also Phase 2 studies exploring disease-modifying therapies. Want me to pull the full details on any of these?

---

**👤 You:**
> "Show me Phase 3 trials related to breast cancer treatment."

**🤖 AI Agent:**
> Here are the Phase 3 breast cancer trials I found. The results include large-scale multi-center studies testing new combination therapies and immunotherapy approaches. Each listing shows the sponsor, enrollment target, and current recruitment status so you can see which ones are still open for participation.

---

**👤 You:**
> "Get me the full details for trial NCT04280705."

**🤖 AI Agent:**
> Here is the complete profile for NCT04280705. The study summary, eligibility criteria, interventions being tested, and enrollment timeline are all included. The trial is sponsored by a major research institution and has multiple collaborating partners.


## ❓ FAQ

**Q: Do I need an API Key or registration?**
No. ClinicalTrials.gov is a fully public service maintained by the US National Library of Medicine. All data is accessible without any authentication.

**Q: What types of studies can I search for?**
The database covers interventional trials (testing drugs, devices, procedures), observational studies, and expanded access programs. You can search across all phases, from early Phase 1 research to post-market Phase 4 surveillance.

**Q: Is the trial recruiting status updated in real time?**
The data reflects what is currently published on the ClinicalTrials.gov database. Sponsors typically update the registry directly, so you will see the latest status logged in their system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clinicaltrialsgov](https://vinkius.com/mcp/clinicaltrialsgov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClinicalTrials.gov** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clinicaltrialsgov` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClinicalTrials.gov** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clinicaltrialsgov": {
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
