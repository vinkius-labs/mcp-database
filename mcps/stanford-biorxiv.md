# Stanford bioRxiv MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-biorxiv)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Search and retrieve preprint research papers in biology and life sciences from the bioRxiv open access repository.

## Description
Connect to the **bioRxiv and medRxiv APIs** — the world's leading preprint servers for biology and health sciences.

### What you can do

- **bioRxiv Preprints** — Browse the latest biology preprints across 25+ categories
- **medRxiv Preprints** — Browse health sciences preprints (clinical, epidemiology, public health)
- **Category Filters** — Neuroscience, genomics, cell biology, cancer, immunology, and more
- **Preprint Details** — Get full metadata including abstracts by DOI
- **Version Tracking** — See how a preprint has been revised over time
- **Publication Tracking** — Discover which preprints have been published in peer-reviewed journals
- **Institution View** — Browse preprints by corresponding author institution
- **Subject Feeds** — Dedicated feeds for neuroscience, genomics, immunology, cell biology, cancer, and epidemiology

### Why preprints matter

Preprints appear **6-12 months before** peer-reviewed publication. This server gives you access to science at the cutting edge — the same day researchers share their findings with the world.

### Who is this for?

- **Biologists** — stay current with your field before journals publish
- **Medical Researchers** — monitor clinical and epidemiological preprints
- **PhD Students** — discover the freshest research in your specialty
- **Science Journalists** — track breaking scientific discoveries


## Available Tools
- **get_preprint**: Searches both bioRxiv and medRxiv. Returns title, authors, corresponding author and institution, date, version, category, abstract, and license. DOI format: "10.1101/2024.01.15.575123".

Get preprint details by DOI
- **get_preprint_versions**: Preprints on bioRxiv/medRxiv can be updated multiple times. This lets you see the full revision history and understand how a manuscript has evolved.

Get all versions of a preprint to track revisions
- **get_published_tracking**: Shows the preprint DOI, published DOI, journal name, and publication date. Essential for understanding the preprint-to-publication pipeline.

Track which preprints have been published in journals
- **get_published_version**: Returns the published DOI, journal citation, and publication date. Essential for finding the final, peer-reviewed version of a preprint you have read.

Find the journal-published version of a preprint
- **get_recent_biorxiv**: Default is 7 days. Essential for staying at the cutting edge of biological research — preprints appear here 6-12 months before peer-reviewed publication.

Get the latest bioRxiv preprints
- **get_recent_medrxiv**: Covers clinical medicine, epidemiology, public health, and health systems research. Critical for monitoring emerging health research before journal publication.

Get the latest medRxiv preprints
- **search_biorxiv**: The bioRxiv API returns preprints in batches of 100. Use the date interval format "YYYY-MM-DD/YYYY-MM-DD" (e.g. "2024-01-01/2024-01-31"). Use cursor for pagination (0, 100, 200, etc.).

Browse bioRxiv preprints by date range
- **search_by_category**: bioRxiv categories include: neuroscience, genomics, bioinformatics, cell_biology, cancer_biology, immunology, microbiology, molecular_biology, biochemistry, genetics, developmental_biology, evolutionary_biology, ecology, plant_biology, physiology, pharmacology, systems_biology, biophysics, synthetic_biology. medRxiv categories: epidemiology, infectious_diseases, public_and_global_health, health_systems, cardiovascular_medicine, oncology, psychiatry, neurology.

Filter preprints by subject category
- **search_by_institution**: Use this to explore what institutions are producing preprints in a given time period. Each preprint includes the corresponding author and their institutional affiliation.

Browse preprints with author institution metadata
- **search_cancer**: Covers tumor biology, oncogenomics, cancer immunology, drug resistance, and experimental therapeutics.

Browse cancer biology preprints
- **search_cell_biology**: Covers cell signaling, organelle biology, cytoskeleton, cell division, stem cells, and cellular mechanisms of disease.

Browse cell biology preprints
- **search_epidemiology**: Covers disease surveillance, outbreak analysis, population health, health policy, and clinical epidemiology. Critical for public health monitoring.

Browse epidemiology and public health preprints
- **search_genomics**: Covers genome sequencing, gene regulation, epigenomics, metagenomics, and computational genomics — core disciplines in modern biology.

Browse genomics and bioinformatics preprints
- **search_immunology**: Covers immune system research, host-pathogen interactions, vaccine development, autoimmune diseases, and immunotherapy.

Browse immunology and microbiology preprints
- **search_medrxiv**: medRxiv covers clinical research, epidemiology, public health, and health policy. Use interval "YYYY-MM-DD/YYYY-MM-DD" format. Results paginated in batches of 100.

Browse medRxiv preprints by date range
- **search_neuroscience**: Neuroscience is one of the largest and most active categories, covering brain research, neural circuits, cognitive science, and neurological disorders.

Browse neuroscience preprints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stanford bioRxiv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest neuroscience preprints"

**🤖 AI Agent:**
> I've retrieved the latest neuroscience preprints from bioRxiv. Recent submissions cover topics including neural circuits, brain imaging, cognitive neuroscience, and neurological disorders.

---

**👤 You:**
> "Has preprint 10.1101/2024.01.15.575123 been published in a journal?"

**🤖 AI Agent:**
> I've checked the publication tracking for this preprint. If published, I'll show the journal DOI, citation, and publication date.

---

**👤 You:**
> "Find the latest genomics preprints from this week"

**🤖 AI Agent:**
> I've retrieved this week's genomics preprints from bioRxiv, including recent work on single-cell sequencing, CRISPR screens, and population genetics.


## ❓ FAQ

**Q: Do I need an API key?**
No. The bioRxiv and medRxiv APIs are completely free and public.

**Q: What is the difference between bioRxiv and medRxiv?**
bioRxiv covers biological sciences (neuroscience, genomics, cell biology, ecology, etc.) while medRxiv covers health sciences (clinical research, epidemiology, public health, health systems).

**Q: Are preprints peer-reviewed?**
No. Preprints are shared before formal peer review. They undergo basic screening but not the full editorial process. This server also tracks which preprints later get published in peer-reviewed journals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-biorxiv](https://vinkius.com/mcp/stanford-biorxiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stanford bioRxiv** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stanford-biorxiv` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stanford bioRxiv** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stanford-biorxiv": {
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
