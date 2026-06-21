# Stanford bioRxiv MCP Server

Search and retrieve preprint research papers in biology and life sciences from the bioRxiv open access repository.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-biorxiv)

## Overview
**Category:** education
**Tools Count:** 16

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


## Installation & Usage

To install and use the **Stanford bioRxiv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-biorxiv](https://vinkius.com/mcp/stanford-biorxiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
