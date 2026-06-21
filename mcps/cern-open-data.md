# CERN Open Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cern-open-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Explore particle physics datasets from the Large Hadron Collider and access open research data from CERN experiments.

## Description
Connect to the **CERN Open Data Portal** and access the world's largest repository of open particle physics data — over 66,000 datasets from the Large Hadron Collider and LEP experiments.

### What you can do

- **Dataset Discovery** — Search across 66,000+ records with powerful filters for experiment (CMS, ATLAS, ALICE, LHCb, DELPHI, OPERA), collision type (pp, e+e−, Pb-Pb), collision energy (7–13.6 TeV), and physics category
- **Physics Categories** — Browse datasets by research topic including Higgs boson, Exotica (Dark Matter, Gravitons, Extra Dimensions, Leptoquarks), B physics, heavy-ion collisions, and more
- **Record Intelligence** — Retrieve complete metadata for any record: abstracts, authors with ORCID, DOI, event counts, file listings with ROOT/EOS URIs, and processing configurations
- **Portal Analytics** — Get comprehensive statistics across all facets: experiments, collision types, energies, file formats, years, and event count distributions
- **Physics Glossary** — Search 1,000+ glossary entries for definitions of particle physics terms, detector components, and analysis techniques
- **Software & Documentation** — Find analysis frameworks, reconstruction software, guides, and supplementary materials needed to reproduce published results

### How it works

1. Subscribe to this server
2. No API key required — the CERN Open Data Portal is a fully public service
3. Start querying particle physics data from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a particle physics research assistant with direct access to LHC collision data. All data is sourced from the official CERN Open Data Portal powered by InvenioRDM.

### Who is this for?

- **Particle Physicists** — discover and access collision datasets, reconstruction configurations, and analysis software without navigating complex web interfaces
- **Data Scientists & ML Researchers** — find labeled physics datasets for machine learning applications in particle identification, anomaly detection, and event classification
- **Educators & Students** — access curated educational datasets and physics glossary entries for teaching and learning particle physics
- **Science Communicators** — retrieve real data from Higgs boson discoveries, Dark Matter searches, and other landmark physics results for accurate reporting


## Available Tools
- **check_cern_opendata_status**: Use this to verify the integration is working correctly before performing data queries. The API uses the InvenioRDM REST framework.

Verify CERN Open Data API connectivity and portal status
- **get_glossary**: Returns term names, definitions, and associated experiments. Covers fundamental particles, detector components, analysis techniques, and physics phenomena. Use this to explain technical physics terms like "luminosity", "transverse momentum", "pseudorapidity", "b-tagging", or "muon spectrometer". Invaluable for science communication and educational contexts.

Search the CERN particle physics glossary for term definitions
- **get_portal_statistics**: ), record types (Dataset, Documentation, Software, Glossary, Supplementaries), data-taking years, keywords, availability status, and event count distributions. This is the single most informative endpoint for understanding the scope and composition of available CERN data.

Get comprehensive CERN Open Data portal statistics and facets
- **get_record_by_doi**: Returns the resolved record ID, title, experiment, type, and direct link if found. Useful when you have a DOI from a publication or reference and need to find the corresponding open dataset. DOIs follow the format "10.7483/OPENDATA.CMS.XXX". Returns a "not found" result if the DOI does not match any record.

Resolve a DOI to a CERN Open Data record
- **get_record**: Returns the full title, abstract, experiment, authors with ORCID identifiers, collision parameters, publication dates, DOI, file distribution summary (number of files, events, size), usage instructions, and a direct link. Use this after finding a record via search to obtain complete details. Example: recid "1" returns the CMS BTau primary dataset.

Get detailed metadata for a specific CERN Open Data record
- **list_categories**: Returns category names and dataset counts. Categories span the full range of particle physics research: Higgs boson searches, exotic particles (Dark Matter, Extra Dimensions, Gravitons), B physics, heavy-ion collisions, and more. Subcategories within Exotica and Higgs Physics provide finer granularity.

List all physics categories and subcategories with dataset counts
- **list_experiments**: Currently includes CMS (the largest contributor with ~52,000 datasets), DELPHI (LEP era), ATLAS, ALICE, LHCb, OPERA (neutrino physics), TOTEM, JADE, and PHENIX. Use this as a starting point to understand what data is available before drilling into specific experiments.

List all available CERN experiments and their dataset counts
- **list_record_files**: Returns filename, size in bytes, checksum, ROOT/EOS URI for direct data access, and file format. Useful for understanding what data is available in a dataset before downloading. Large datasets may contain hundreds of ROOT files. Example: record 1 contains AOD format files from CMS BTau data.

List all data files in a CERN Open Data record
- **search_by_category**: Major categories include: Exotica (~13,000 datasets, including Dark Matter, Extra Dimensions, Gravitons, Heavy Fermions, Leptoquarks), Higgs Physics (~10,400, Standard Model and Beyond Standard Model), Higgs (~10,700), Beyond 2 Generations (~1,600), 2 Fermion (~1,200), B physics and Quarkonia (~500), 4 Fermion (~380), Heavy-Ion Physics (~220). Some categories have subcategories — use the subcategory parameter for more precise filtering.

Search datasets filtered by physics category
- **search_by_collision_energy**: Available energies include: 13TeV (~50,500 datasets, LHC Run 2), 181-210 GeV (~11,700, LEP2), 7TeV (~1,100, LHC Run 1), 8TeV (~900, LHC Run 1), 5.02TeV (~310, heavy-ion), 2.76TeV (~120, heavy-ion), 130-140 GeV (~120, LEP), 13.6TeV (LHC Run 3). The vast majority of data comes from 13 TeV proton-proton collisions at the LHC.

Search datasets filtered by collision energy
- **search_by_collision_type**: Available collision types: pp (proton-proton, ~52,000 datasets), e+e- (electron-positron, ~12,700), Pb-Pb (lead-lead, ~140), pPb (proton-lead, ~140). Proton-proton collisions from the LHC dominate the dataset. Electron-positron data comes primarily from the LEP era (DELPHI). Use this to focus on a specific collision topology.

Search datasets filtered by particle collision type
- **search_by_experiment**: Available experiments include CMS (~52,000 datasets), DELPHI (~12,700), ATLAS (~160), ALICE (~150), LHCb (~108), OPERA (~900), and TOTEM. Combine with a text query for targeted searches within an experiment. This is the fastest way to scope results to a single collaboration.

Search datasets filtered by a specific LHC experiment
- **search_datasets**: Supports full-text queries combined with filters for experiment, collision type, collision energy, physics category, file type, and year. Returns paginated results with metadata including record ID, title, abstract, event counts, file sizes, and direct links. Use this as the primary discovery tool for finding specific physics data. Example queries: "Higgs boson", "dark matter", "top quark pair production".

Search CERN Open Data datasets with full-text query and filters
- **search_documentation**: Returns document titles, abstracts, subtypes (Guide, Policy, About, Activities, Authors, Report, Help, Stripping), and direct links. Use this to find instructions on how to use specific datasets, understand detector configurations, or learn about data processing workflows.

Search CERN guides, policies, and documentation
- **search_software**: Returns software title, description, associated experiment, and subtypes (Analysis, Framework, Tool, Validation, Workflow). Use this to find reconstruction software, analysis frameworks like CMSSW, or specific analysis code associated with published physics results.

Search CERN analysis software, frameworks, and tools
- **search_supplementaries**: These ~5,900 records provide the technical context needed to reproduce physics analyses. Filter by subtype to find specific configuration types. Essential for researchers reproducing or extending published analyses.

Search CERN supplementary materials and configurations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CERN Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the available experiments and how many datasets each one has on CERN Open Data."

**🤖 AI Agent:**
> I've retrieved the experiment list from CERN Open Data. There are 9 experiments with published datasets: CMS leads with 51,955 datasets, followed by DELPHI (12,727), OPERA (904), ATLAS (159), ALICE (153), LHCb (108), TOTEM (1), JADE (1), and PHENIX (1). The total repository contains 66,009 datasets. Would you like me to search within a specific experiment?

---

**👤 You:**
> "Search for Dark Matter datasets from the CMS experiment at 13 TeV."

**🤖 AI Agent:**
> I've found Dark Matter datasets from CMS at 13 TeV. The search returned simulated datasets in NanoAODSIM format containing dark matter signal samples. Each record includes event counts ranging from 50,000 to 500,000 events, with file sizes in ROOT format. These datasets are commonly used for mono-jet, mono-photon, and missing transverse energy analyses. Would you like the full file listing for any specific record?

---

**👤 You:**
> "What does 'luminosity' mean in particle physics? Check the CERN glossary."

**🤖 AI Agent:**
> According to the CERN physics glossary, luminosity is a measure of the number of collisions that can be produced in a particle accelerator. It is one of the most important parameters of an accelerator, directly related to the number of events observed. Integrated luminosity (measured in inverse femtobarns, fb⁻¹) quantifies the total data collected during a run period. Higher luminosity means more collision events and greater chances of observing rare processes like Higgs boson production.


## ❓ FAQ

**Q: Do I need an API key to use this server?**
No. The CERN Open Data Portal API is completely public and requires no authentication. Simply subscribe to this server and enter any placeholder value in the API key field to start querying particle physics datasets immediately.

**Q: What kind of data can I access from CERN?**
You can access over 66,000 datasets from major LHC experiments (CMS, ATLAS, ALICE, LHCb) and legacy experiments (DELPHI, OPERA). This includes real collision data, Monte Carlo simulations, derived datasets, analysis software, physics glossary entries, and detailed documentation. Data covers Higgs boson searches, Dark Matter studies, exotic particle searches, heavy-ion physics, and more.

**Q: Can I use CERN data for machine learning projects?**
Absolutely. CERN provides labeled datasets specifically designed for ML applications, including particle identification, jet classification, event reconstruction, and anomaly detection. Use the search tools with queries like 'machine learning' or filter by file type 'csv' or 'nanoaodsim' to find ML-ready formats. The CMS experiment alone has published thousands of simulated datasets with known physics labels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cern-open-data](https://vinkius.com/mcp/cern-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CERN Open Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cern-open-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CERN Open Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cern-open-data": {
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
