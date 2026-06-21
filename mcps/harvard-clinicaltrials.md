# Harvard ClinicalTrials MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvard-clinicaltrials)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/harvard-clinicaltrials-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/harvard-clinicaltrials-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search and analyze clinical trial data from Harvard and ClinicalTrials.gov for research, drug development, and healthcare innovation.

## Description
Connect to the **ClinicalTrials.gov API v2** — the largest database of clinical studies worldwide, maintained by the U.S. National Library of Medicine.

### What you can do

- **Study Search** — Search 400K+ clinical trials from 220+ countries
- **Condition Filter** — Find trials for specific diseases (cancer, diabetes, Alzheimer's)
- **Intervention Filter** — Search by drug, device, or therapy name
- **Sponsor Search** — Find trials by organization (Pfizer, NIH, Roche)
- **Phase Filter** — Filter by Phase 1-4 to track drug development stages
- **Recruiting** — Find trials currently enrolling participants
- **Location** — Search by city or country for accessible trials
- **FDA Regulated** — Filter for FDA-regulated drug and device trials
- **Pediatric** — Find trials including children
- **Rare Diseases** — Discover research for orphan conditions
- **Results** — Get outcome data from completed studies

### Who is this for?

- **Medical Researchers** — systematic reviews and evidence synthesis
- **Clinicians** — find trial evidence for treatment decisions
- **Patients** — discover trials they may be eligible for
- **Pharma Professionals** — competitive landscape and pipeline analysis


## Available Tools
- **get_api_version**: gov API version and the timestamp of the most recent data update. Useful for verifying data currency and API availability.

Get API version and data timestamp
- **get_study**: g. "NCT04368728"). Returns title, status, phase, enrollment, conditions, interventions, eligibility criteria, sponsor, and study locations.

Get clinical trial details by NCT ID
- **get_study_results**: Not all trials report results — this is most useful for completed Phase 2-4 studies.

Get primary outcome results for a trial
- **get_study_timeline**: Essential for understanding the progress and currency of a study.

Get the complete timeline of a clinical trial
- **search_by_condition**: Examples: "diabetes", "breast cancer", "Alzheimer disease", "COVID-19", "depression", "hypertension".

Search trials by medical condition
- **search_by_intervention**: Examples: "pembrolizumab", "metformin", "radiation therapy", "cognitive behavioral therapy".

Search trials by drug or treatment
- **search_by_location**: Essential for finding trials accessible to patients in a particular area.

Search trials by geographic location
- **search_by_phase**: Phase values: "PHASE1", "PHASE2", "PHASE3", "PHASE4", "EARLY_PHASE1". Phase 3 trials are the largest and most definitive, while Phase 1 trials focus on safety.

Search trials by study phase
- **search_by_sponsor**: Examples: "Pfizer", "National Cancer Institute", "Roche", "Novartis", "NIH".

Search trials by sponsoring organization
- **search_completed**: Completed trials are more likely to have published results and outcomes data.

Search completed clinical trials
- **search_device_trials**: Covers diagnostic devices, surgical tools, implants, and digital health technologies.

Search medical device clinical trials
- **search_fda_regulated**: S. Food and Drug Administration. These trials follow the most rigorous regulatory standards.

Search FDA-regulated drug trials
- **search_pediatric**: Essential for pediatricians, child health researchers, and parents seeking trials for children.

Search pediatric clinical trials
- **search_rare_diseases**: Examples: "cystic fibrosis", "sickle cell disease", "Huntington disease", "amyotrophic lateral sclerosis".

Search rare disease clinical trials
- **search_recruiting**: Essential for patients seeking to enroll in trials or researchers tracking active studies.

Search for currently recruiting studies
- **search_studies**: gov database of over 400,000 clinical studies from 200+ countries. Returns NCT IDs, titles, status, phases, sponsors, conditions, interventions, and locations.

Search 400K+ clinical trials worldwide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvard ClinicalTrials** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find recruiting Phase 3 trials for breast cancer immunotherapy"

**🤖 AI Agent:**
> I've found Phase 3 clinical trials for breast cancer immunotherapy that are currently recruiting participants, including studies testing checkpoint inhibitors and combination therapies.

---

**👤 You:**
> "Search for Alzheimer's disease trials sponsored by NIH in Boston"

**🤖 AI Agent:**
> I've found NIH-sponsored Alzheimer's disease trials in Boston, including studies on amyloid-targeting therapies and cognitive interventions at major research hospitals.

---

**👤 You:**
> "Find pediatric clinical trials for cystic fibrosis"

**🤖 AI Agent:**
> I've searched for pediatric cystic fibrosis trials, including CFTR modulator studies and gene therapy trials enrolling children and adolescents.


## Installation & Usage

To install and use the **Harvard ClinicalTrials** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvard-clinicaltrials](https://vinkius.com/mcp/harvard-clinicaltrials)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
